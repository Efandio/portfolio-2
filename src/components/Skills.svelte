<script>
    const ui_ux_skills = [
        'User Research',
        'Wireframe & Prototyping',
        'User Interfaces (UI) Design',
        'Usability Principles',
        'Information Architecture',
        'Design System'
    ]

    const skill = [
        {
            title: 'Soft Skills',
            skills: [
                'User Empathy',
                'Problem Solving',
                'Collaboration & Communication',
                'Critical Thinking',
                'Rapid Learning & Adaptability',
            ],
        },
        {
            title: 'Frontend Development',
            skills: [
                'HTML, CSS (Flexbox, CSS Grid)',
                'Tailwind CSS',
                'JavaScript/TypeScript',
                'React/Vue',
            ],
        },
        {
            title: 'Design Tool',
            skills: [
                'Figma',
            ],
        },
    ]
</script>

<section id="skills" class="w-full h-full pt-30 flex flex-col gap-3 px-4 md:px-10">
    <h3 class="text-accent font-semibold italic text-xl border-b border-accent w-fit pr-4">
        Skills
    </h3>
    <div class="w-full h-full flex flex-col gap-10">
        <div class="w-full h-full flex justify-between items-center gap-4 border-b border-primary pb-10 rounded-md">
            <div class="w-[20vw] h-full text-primary font-semibold text-xl">
                    UI/UX Design
            </div> 
            <div class="w-[80vw] h-full grid md:grid-cols-2 gap-3 justify-items-center">
                {#each ui_ux_skills as skills }
                    <p class="bg-accent text-background w-full text-center py-2 rounded-lg font-medium flex items-center justify-center text-sm">{skills}</p>
                {/each}
            </div>
        </div>
        <div class="w-full h-full grid grid-cols-2 md:grid-cols-3 justify-between items-center gap-10">
            {#each skill as skills }
                <div class="w-full h-70 flex flex-col gap-3 items-start">
                    <h4 class="text-primary">{skills.title}</h4>
                    {#each skills.skills as skill }
                        <p class="bg-accent w-fit text-background text-center px-4 py-2 rounded-lg font-medium flex items-center justify-center text-sm">{skill}</p>
                    {/each}
                </div>
            {/each}
        </div>
    </div>
</section>