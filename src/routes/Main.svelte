<script>
    import foto from '$lib/images/Offline Leadership UI.svg';
    import asset1 from '$lib/images/homepage_asset1.png';
    import asset2 from '$lib/images/homepage_asset2.png';
    import asset3 from '$lib/images/homepage_asset3.png';
    import asset4 from '$lib/images/homepage_asset4.png';
    import asset5 from '$lib/images/bxs-bank 1.svg';
    import asset6 from '$lib/images/bx-book-open 1.svg';
    import asset7 from '$lib/images/bx-chat 1.svg';
    import glints from '$lib/images/glints.png';
    import JungleVentures from '$lib/images/Jungle Ventures.jpg';
    import mhv from '$lib/images/MHV.png';
    import { goto } from '$app/navigation';
</script>
<div class="section one bg-black py-5">
  <div class="text-center text-neutral-100 text-4xl font-black font-primary">Where Future Leaders Unlock Their Potentials</div>
  <div class="text-center text-neutral-100 text-2xl font-primary">TASLA is a dedicated scholarship to help you unlock your leadership potentials.</div>
  <div class="flex items-center justify-center rounded-md">
    <img src={foto} alt="TASLA Offline Leadership Program at UI" class="py-4 bg-opacity-50">
  </div>
</div>

<div class="h-[75px] transition bg-gradient-to-b from-black to-gray-700 shadow"></div>

<div class="section two bg-gray-700 shadow px-10">
  <div class="py-1 text-left text-white text-4xl font-black font-primary">Experience leadership by practically doing it</div>
  <div class="py-1 text-left text-white text-xl font-primary">TASLA helps unlocking your leadership potentials through viral leadership, you will be exposed to maintain 4 of the following programs.</div>
  <div class="grid grid-cols-4 py-10">
    <div class="w-3/4 mx-auto">
      <div class="relative aspect-w-3 aspect-h-4">
        <img src="{asset1}" alt="Mentorship Program" class="object-cover w-full h-full">
        <div class="absolute inset-0 bg-black bg-opacity-50 flex justify-center items-center">
          <span class="text-white text-2xl text-center font-bold font-primary">Mentorship Program</span>
        </div>
      </div>
    </div>
    <div class="w-3/4 mx-auto">
      <div class="relative aspect-w-3 aspect-h-4">
        <img src="{asset2}" alt="primarynship Placement" class="object-cover w-full h-full">
        <div class="absolute inset-0 bg-black bg-opacity-50 flex justify-center items-center">
          <span class="text-white text-2xl text-center font-bold font-primary">Internship Placement</span>
        </div>
      </div>
    </div>
    <div class="w-3/4 mx-auto">
      <div class="relative aspect-w-3 aspect-h-4">
        <img src="{asset3}" alt="Leadership Training" class="object-cover w-full h-full">
        <div class="absolute inset-0 bg-black bg-opacity-50 flex justify-center items-center">
          <span class="text-white text-2xl text-center font-bold font-primary">Leadership Training</span>
        </div>
      </div>
    </div>
    <div class="w-3/4 mx-auto">
      <div class="relative aspect-w-3 aspect-h-4">
        <img src="{asset4}" alt="Community Service" class="object-cover w-full h-full">
        <div class="absolute inset-0 bg-black bg-opacity-50 flex justify-center items-center">
          <span class="text-white text-2xl text-center font-bold font-primary">Sharing Session Program</span>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="section three bg-gray-700 shadow py-5 px-10">
  <div class=" text-white text-4xl font-black font-primary">What are the benefits of being a TASLA scholar?</div>
  <div class=" break-all text-white text-xl font-normal font-primary">Besides of being exposed to maintain our leadership program, there are several benefits as part of our scholarship.</div>
  <div class="grid grid-cols-3 gap-x-5 px-48 py-10">
    <div class="w-[78px] h-[74px] bg-gradient-to-b from-cyan-300 to-indigo-600 rounded-[10px]">
      <img src="{asset5}" alt="TASLA Offline Leadership Program at UI" class="w-[78px] h-[74px]">
      <div class="py-4 w-[291px] h-9 text-white text-2xl font-bold font-primary">Full tuition fee coverage</div>
      <div class="break-all py-4 w-[354px] h-24 text-white text-xl font-normal font-primary">TASLA is dedicated to fully cover their scholars tuition fee. The tuition fee will be directly transferred to the corresponding scholar’s university.</div>
    </div>
    <div class="w-[78px] h-[74px] bg-gradient-to-b from-cyan-300 to-indigo-600 rounded-[10px]">
      <img src="{asset6}" alt="TASLA Offline Leadership Program at UI" class="w-[78px] h-[74px]">
      <div class="py-4 w-[291px] h-9 text-white text-2xl font-bold font-primary">Books Allowance </div>
      <div class="break-all py-4 w-[354px] h-24 text-white text-xl font-normal font-primary">As part of the scholarship, TASLA scholars will obtain books allowance that will be granted for every semester of their study.</div>
    </div>
    <div class="w-[78px] h-[74px] bg-gradient-to-b from-cyan-300 to-indigo-600 rounded-[10px]">
      <img src="{asset7}" alt="TASLA Offline Leadership Program at UI" class="w-[78px] h-[74px]">
      <div class="py-4 w-[291px] h-9 text-white text-2xl font-bold font-primary">Networks</div>
      <div class="break-all py-4 w-[393px] h-24 text-white text-xl font-normal font-primary">TASLA is has a network of several big tech companies, often we have the opportunities to invites CEOs to help mentor the scholars about leaderships.</div>
    </div>
  </div>
</div>

<div class="h-[150px] transition bg-gradient-to-b from-gray-700 to-black shadow"></div>

<div class="section four bg-black px-10 py-5">
  <div class=" py-1 text-white text-4xl font-black font-primary">How does the TASLA organization looks like?</div>
  <div class=" py-3 text-white text-xl font-normal font-primary">Our scholarships' structure have 3 main roles inside of it.</div>
  <div class=" py-1 text-white text-4xl font-black font-primary">The Board Members</div>
  <div class=" py-3 text-white text-xl font-normal font-primary">The Board Members are those who supervised every TASLA proposed activity. About every month, TASLA scholars held a meeting to report their progresses and achievements for the month.</div>
  <div class=" py-1 text-white text-4xl font-black font-primary">The Community Manager</div>
  <div class=" py-3 text-white text-xl font-normal font-primary">The community manager is there to help and guide TASLA scholars for any TASLA related activity.</div>
  <div class=" py-1 text-white text-4xl font-black font-primary">The scholars</div>
  <div class=" py-3 text-white text-xl font-normal font-primary">Those who obtain the TASLA scholarships, every cohort has different amount of students selected as TASLA scholars. As for now, the application is only open for UI and ITB STEM students.</div>
  <br>
  <button class="bg-gradient-to-b from-cyan-300 to-indigo-600 text-white text-xl font-bold font-primary rounded-md py-3 px-4" on:click={() => goto("/our-organization")}>Learn more about the organization</button>
</div>

<div class="h-[150px] transition bg-gradient-to-b from-black to-gray-700 shadow"></div>

<div class="bg-gray-700 shadow py-4">
  <h2 class="text-center text-white text-2xl md:text-3xl lg:text-4xl font-bold">Who are our sponsors?</h2>
  <div class="flex flex-row justify-center items-center gap-4 md:gap-6 p-4 md:p-8">
    <div class="flex justify-center items-center  rounded-lg shadow-lg w-1/6 p-4">
      <img class="h-full w-full object-contain" src="{glints}" alt="Glints" />
    </div>
    <div class="flex justify-center items-center  rounded-lg shadow-lg w-1/6 p-4">
      <img class="h-full w-full object-contain" src="{JungleVentures}" alt="Jungle Ventures" />
    </div>
    <div class="flex justify-center items-center  rounded-lg shadow-lg w-1/3 p-4">
      <img class="h-full w-full object-contain" src="{mhv}" alt="Monk's Hill Ventures" />
    </div>
  </div>
  <div class="text-center">
    <button class="bg-gradient-to-b from-cyan-300 to-indigo-600 text-white text-xl font-bold font-primary rounded-md py-3 px-4" on:click={() => goto("/sponsors")}>
      Learn more about TASLA
    </button>
  </div>
</div>

<div class="h-[150px] transition bg-gradient-to-b from-gray-700 to-black shadow"></div>

<div class="bg-black flex flex-col px-5 py-5">
	<div class="text-white text-4xl font-black font-primary py-5">Interested to be our sponsor?</div>
	<div class="text-justify text-white text-xl font-normal font-primary py-5">By being TASLA sponsor, you are helping Indonesia to nurture more future leaders. A lot of our Alumni has proven a significant contribution throughout the Indonesia ecosystem. This can be part of your contribution too!</div>
	<div class="text-white text-4xl font-black font-primary py-5">Contact us!</div>
	<div class="text-white text-xl font-black font-primary py-5">Email: admin@csleaders.com<br/>Instagram: tasla_org<br/>Our Contact Form</div>
</div>