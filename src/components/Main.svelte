<script>
     import Step from "./Step.svelte";
     let steps= [
        {name:'SmolGems Store', icon: 'fa-solid fa-cart-shopping'},
        {name: 'Ultimate Todos', icon: 'fa-solid fa-list-check'},
        {name: 'Pokedex', icon:'fa-solid fa-diagram-project'},
     ];

     let benefits=[
        {name:'An Engineering Student', description:'I am an engineering student pursuing my Btech degree from BVCOE in Informataional Technology and will be passing out in year 2024.'},
        {name:'A Quick Learner', description:'I am a quick learner and aspire to learn new things and technologies and grow myself as well as my skillset alonside.'},
        {name:'A Good Communicator', description:'Communication is the key and it is a paramount  value of mine. I believe in transparency and cinstructive communication above all else. This helps me develop a deep relationships and ensures my effectiveness and productivity in any work space with any team.'},
     ]

</script>
<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 mid:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
            Hello! I'm <span class="text-violet-400">Bhanu</span> VK
            <br> An Engineering <span class="text-violet-400">Student</span>
        </h2>
        <p class="text-base sm:text-lg md:text-xl">My
            <span class="text-violet-400">favourite tech</span> includes Java, HTML, CSS, JavaScript, ReactJS, AWS(Amazon Web Services) and many more!
        </p>
        <a class="blueShadow mx-auto lg:ar-auto lg:ml-0 text-base sm:text-lg md:text-xl relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" href="https://www.instagram.com/vkbhanu/"
        target="_blank" >
            <div class="absolute top-0 right-full w-full h-full bg-voilet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"/>
            <h4 class="relative z-9">Get in Touch &rarr;</h4>
        </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img src="images/profile_image.png" alt="Profile image"
            class="object-cover z-[2] max-h-[70vh]"/>
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of My Projects
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="text-violet-400">see</span> my work?
            </h3>
        </div>
        <a href="https://youtu.be/dQw4w9WgXcQ?si=w4rnNGBUvssnf9jm" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration 200">
            <i class="fa-regular fa-circular-play"></i>
            <p>Watch the Video</p>
            </a>
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-18">
                <Step step={steps[0]}>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. odio tenetur eveniet?</p>
                </Step>
                <Step step={steps[1]}>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. odio tenetur eveniet?</p>
                </Step>
                <Step step={steps[2]}>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. odio tenetur eveniet?</p>
                </Step>
            </div>
    </section>
    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl">Want to Know more?</h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="text-violet-400">about </span>me. 
            </h3>
        </div>
        <p class="mx-auto font-semibold text-lg sm:text-xl md:text-2xl">I am. . .</p>
        <div class="flex flex-col gap-20 w-full max-w-[800px]">
            {#each benefits as benefit, index}
            <div class="flex gap-6 sm:gap-8">
                <p class="text-4xl sm:text-5xl md:text-6xl tex-slate-500 font-semibold">
                    0{index + 1}
                </p>
                <div class="flex flex-col gap-6 sm:gap-8">
                    <h3 class="text-2xl sm:text-3xl md:text-5xl">
                        {benefit.name}
                    </h3>
                    <p>{benefit.description}</p>
                </div>
            </div>
            {/each}
        </div>
        <h5 class="text-2xl sm:text-3xl font-semibold text-center">The <span class="text-violet-400">Complete</span> Package</h5>
        <div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr class="">
                        <th/>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th class="whitespace-nowrap bg-violet-700 text-white p-4 px-8">Me</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font semibold text-sm whitespace-nowrap">Dedication</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font semibold text-sm whitespace-nowrap">Critical Thinking</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font semibold text-sm whitespace-nowrap">Interpersonal Skills</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font semibold text-sm whitespace-nowrap">Programming Ability</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not Invest?</p>
    </section>
</main>