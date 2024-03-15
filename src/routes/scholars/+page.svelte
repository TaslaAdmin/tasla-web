<script>
// @ts-nocheck

    import { onMount } from 'svelte';
    import afterGradChart from '$lib/images/after-graduation.png';
  
    /**
   * @type {any[]}
   */
    let scholars = [];
    let scholarsByYear = {};
    let searchQuery = '';
  
    onMount(async () => {
      scholars = [
        { id: 1, name: 'Affan Dhia', year: '2015', imageUrl: '/listOfScholars/Affan-Dhia.jpg' },
        { id: 2, name: 'Aldi Fahrezi', year: '2015', imageUrl: '/listOfScholars/Aldi-Fahrezi.jpg' },
        { id: 3, name: 'David Theo', year: '2015', imageUrl: '/listOfScholars/David-Theo.jpg' },
        { id: 4, name: 'Fachrur Rozi', year: '2015', imageUrl: '/listOfScholars/Fachrur-Rozi.jpg' },
        { id: 5, name: 'Fahmi', year:'2015', imageUrl: '/listOfScholars/Fahmi.jpg'},
        { id: 6, name: 'Firman Hadi', year: '2015', imageUrl: '/listOfScholars/Firman-Hadi.jpg' },
        { id: 7, name: 'Nella Zabrina', year: '2016', imageUrl: '/listOfScholars/Nella-Zabrina.jpg' },
        { id: 8, name: 'Tirta Abimanyu', year: '2016', imageUrl: '/listOfScholars/Tirta-Abimanyu.jpg' },
        { id: 9, name: 'Valentina', year: '2016', imageUrl: '/listOfScholars/Valentina.jpg' },
        { id: 10, name: 'Windi Chandra', year:'2016', imageUrl: '/listOfScholars/Windi-Chandra.jpg'},
        { id: 11, name: 'Khatya Puteri', year: '2017', imageUrl: '/listOfScholars/Khatya-Puteri.jpg' },
        { id: 12, name: 'Muhammad Irfan', year: '2017', imageUrl: '/listOfScholars/Muhammad-Irfan.jpg' },
        { id: 13, name: 'Abdurrafi Arief', year: '2018', imageUrl: '/listOfScholars/Abdurrafi-Arief.jpg' },
        { id: 14, name: 'Khadijah Rizqy', year: '2018', imageUrl: '/listOfScholars/Khadijah-Rizqy.jpg' },
        { id: 15, name: 'Michel Fang', year:'2018', imageUrl: '/listOfScholars/Michel-Fang.jpg'},
        { id: 16, name: 'Tolhas Jonathan', year:'2018', imageUrl: '/listOfScholars/Tolhas-Jonathan.jpg'},
        { id: 17, name: 'Priyanty Nurul Fatimah', year: '2019', imageUrl: '/listOfScholars/Priyanti-Nurul.jpeg' },
        { id: 18, name: 'James Chandra', year:'2019', imageUrl: '/listOfScholars/James-Chandra.png'},
        { id: 19, name: 'Dennis Al Baihaqi Walangadi', year:'2019', imageUrl: '/listOfScholars/Dennis-Al.png'},
        { id: 20, name: 'Patrick Amadeus Irawan', year:'2020', imageUrl: '/listOfScholars/Patrick-Amadeus.jpeg'},
        { id: 21, name: 'Alya Astrid Shakila', year: '2020', imageUrl: '/listOfScholars/Alya-Astrid.jpeg' },
        { id: 22, name: 'Muhammad Sulthan Mazaya', year: '2020', imageUrl: '/listOfScholars/Muhammad-Sulthan.jpeg' },
        { id: 23, name: 'Elisha Rachma Salsabila', year: '2021', imageUrl: '/listOfScholars/Elisha-Rachma.jpg' },
        { id: 24, name: 'Yasmina Ashfa Zahidah', year: '2021', imageUrl: '/listOfScholars/Yasmina-Ashfa.jpg' },
        { id: 25, name: 'Lim Bodhi Wijaya', year:'2022', imageUrl: '/listOfScholars/Lim-Bodhi.jpg'},
      ];
  
      scholarsByYear = scholars.reduce((acc, scholar) => {
        if (!acc[scholar.year]) {
          acc[scholar.year] = [];
        }
        acc[scholar.year].push(scholar);
        return acc;
      }, {});
    });
  
    $: filteredScholarsByYear = searchQuery
      ? Object.keys(scholarsByYear).reduce((acc, year) => {
          // @ts-ignore
          const filtered = scholarsByYear[year].filter((scholar) =>
            scholar.name.toLowerCase().includes(searchQuery.toLowerCase())
          );
          // @ts-ignore
          if (filtered.length) acc[year] = filtered;
          return acc;
        }, {})
      : scholarsByYear;
  </script>
  
  <div class="bg-black min-h-screen py-10 px-5">
    <div class="rounded-lg shadow-xl overflow-hidden flex mb-10"> 
      <div class="p-6 space-y-4 w-full"> 
        <div class="text-white text-4xl font-bold font-primary">Our scholars track record</div>
        <div class="text-white text-justify text-xl font-normal font-primary"> 
          Our scholars and alumni are all around the world, shaping the industry they are working on with their leadership capacity. Currently, 27% of the Alumni are working overseas, 46% of them are working with a local company (Indonesian company), and 27% of them are pursuing master degree.
        </div>
      </div>
      <div class="flex items-center w-1/2">
        <img src={afterGradChart} alt="TASLA Alumni Chart"/> 
      </div>
    </div>
  
    <div class="flex justify-between items-center mb-10">
      <div class="text-white text-4xl font-black font-primary">Our scholars database</div>
      <div class="relative w-64">
        <input
          class="w-full h-10 pl-2 pr-10 rounded bg-white"
          type="search"
          placeholder="Search..."
          bind:value="{searchQuery}">
        <div class="absolute inset-y-0 right-0 flex items-center pr-2">
          <svg class="h-6 w-6 fill-current text-gray-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
          </svg>
        </div>
      </div>
    </div>
  
    <!-- Displaying scholars grouped by year -->
    {#each Object.keys(filteredScholarsByYear) as year (year)}
      <div class="mb-8">
        <h2 class="text-2xl text-white font-bold mb-4">{year}</h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
          {#each filteredScholarsByYear[year] as scholar (scholar.id)}
            <div class="bg-gray-800 rounded-lg overflow-hidden shadow">
              <img class="w-full h-48 object-cover" src={scholar.imageUrl} alt={scholar.name} />
              <div class="text-white p-4">
                <h3 class="text-lg font-semibold">{scholar.name}</h3>
                <p>{scholar.year}</p>
              </div>
            </div>
          {/each}
        </div>
      </div>
    {/each}
  </div>