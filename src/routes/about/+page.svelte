<script lang="ts">
    import { page } from '$app/stores';
    import { onMount } from 'svelte';
    import team from './team.js'; // Assuming you have a team.json file with team member data
    // This will run when the component is mounted
    onMount(() => {
        document.title = 'About Us - Not So Boring Startup';
    });
    </script>
<div class="relative flex size-full min-h-screen flex-col bg-gray-50 group/design-root overflow-x-hidden" style='font-family: "Space Grotesk", "Noto Sans", sans-serif;'>
    <div class="layout-container flex h-full grow flex-col">
    
    <div class="px-40 flex flex-1 justify-center py-5">
        <div class="layout-content-container flex flex-col max-w-[960px] flex-1">
        <div class="flex flex-wrap justify-between gap-3 p-4"><p class="text-[#101418] tracking-light text-[32px] font-bold leading-tight min-w-72">About Us</p></div>
        <p class="text-[#101418] text-base font-normal leading-normal pb-3 pt-1 px-4">
            At Not So Boring Startup, we're on a mission to empower individuals and teams to achieve their goals with innovative software solutions. Our journey began with a
            simple idea: to create tools that are both powerful and easy to use, making technology accessible to everyone.
        </p>
        <h2 class="text-[#101418] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">Our Values</h2>
        <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
            <div class="flex flex-1 gap-3 rounded-lg border border-[#d4dbe2] bg-gray-50 p-4 flex-col">
            <div class="text-[#101418]" data-icon="Target" data-size="24px" data-weight="regular">
                <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                <path
                    d="M221.87,83.16A104.1,104.1,0,1,1,195.67,49l22.67-22.68a8,8,0,0,1,11.32,11.32l-96,96a8,8,0,0,1-11.32-11.32l27.72-27.72a40,40,0,1,0,17.87,31.09,8,8,0,1,1,16-.9,56,56,0,1,1-22.38-41.65L184.3,60.39a87.88,87.88,0,1,0,23.13,29.67,8,8,0,0,1,14.44-6.9Z"
                ></path>
                </svg>
            </div>
            <div class="flex flex-col gap-1">
                <h2 class="text-[#101418] text-base font-bold leading-tight">Innovation</h2>
                <p class="text-[#5c738a] text-sm font-normal leading-normal">We constantly seek new and creative ways to solve problems and improve our products.</p>
            </div>
            </div>
            <div class="flex flex-1 gap-3 rounded-lg border border-[#d4dbe2] bg-gray-50 p-4 flex-col">
            <div class="text-[#101418]" data-icon="Users" data-size="24px" data-weight="regular">
                <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                <path
                    d="M117.25,157.92a60,60,0,1,0-66.5,0A95.83,95.83,0,0,0,3.53,195.63a8,8,0,1,0,13.4,8.74,80,80,0,0,1,134.14,0,8,8,0,0,0,13.4-8.74A95.83,95.83,0,0,0,117.25,157.92ZM40,108a44,44,0,1,1,44,44A44.05,44.05,0,0,1,40,108Zm210.14,98.7a8,8,0,0,1-11.07-2.33A79.83,79.83,0,0,0,172,168a8,8,0,0,1,0-16,44,44,0,1,0-16.34-84.87,8,8,0,1,1-5.94-14.85,60,60,0,0,1,55.53,105.64,95.83,95.83,0,0,1,47.22,37.71A8,8,0,0,1,250.14,206.7Z"
                ></path>
                </svg>
            </div>
            <div class="flex flex-col gap-1">
                <h2 class="text-[#101418] text-base font-bold leading-tight">Collaboration</h2>
                <p class="text-[#5c738a] text-sm font-normal leading-normal">
                We believe in the power of teamwork and strive to create a collaborative environment for our users and employees.
                </p>
            </div>
            </div>
            <div class="flex flex-1 gap-3 rounded-lg border border-[#d4dbe2] bg-gray-50 p-4 flex-col">
            <div class="text-[#101418]" data-icon="ShieldCheck" data-size="24px" data-weight="regular">
                <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                <path
                    d="M208,40H48A16,16,0,0,0,32,56v58.78c0,89.61,75.82,119.34,91,124.39a15.53,15.53,0,0,0,10,0c15.2-5.05,91-34.78,91-124.39V56A16,16,0,0,0,208,40Zm0,74.79c0,78.42-66.35,104.62-80,109.18-13.53-4.51-80-30.69-80-109.18V56H208ZM82.34,141.66a8,8,0,0,1,11.32-11.32L112,148.68l50.34-50.34a8,8,0,0,1,11.32,11.32l-56,56a8,8,0,0,1-11.32,0Z"
                ></path>
                </svg>
            </div>
            <div class="flex flex-col gap-1 justify-center">
                <h2 class="text-[#101418] text-base font-bold leading-tight">Integrity</h2>
                <p class="text-[#5c738a] text-sm font-normal leading-normal">We are committed to honesty, transparency, and ethical practices in all our endeavors.</p>
            </div>
            </div>
        </div>
        <h2 class="text-[#101418] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">Our Team</h2>
        <div class="grid gap-3 p-4 grid-cols-[repeat(auto-fit,minmax(158px,1fr))]">
            {#each team as member}
            <div class="flex flex-col gap-3 text-center justify-center items-center pb-3">
                <div class="px-4">
                    <div
                        class="w-20 h-20 rounded-full overflow-hidden bg-cover bg-center bg-no-repeat aspect-square rounded-full"
                        style='background-image: url({member.image});'
                    ></div>
                </div>
                <div>
                    <p class="text-[#101418] text-base font-medium leading-normal">{member.name}</p>
                    <p class="text-[#5c738a] text-sm font-normal leading-normal">{member.role}</p>
                </div>
            </div>
            {/each}
        </div>
        <h2 class="text-[#101418] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">Our History</h2>
        <div class="grid grid-cols-[40px_1fr] gap-x-2 px-4">
            <div class="flex flex-col items-center gap-1 pt-3">
            <div class="text-[#101418]" data-icon="Buildings" data-size="24px" data-weight="regular">
                <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                <path
                    d="M240,208H224V96a16,16,0,0,0-16-16H144V32a16,16,0,0,0-24.88-13.32L39.12,72A16,16,0,0,0,32,85.34V208H16a8,8,0,0,0,0,16H240a8,8,0,0,0,0-16ZM208,96V208H144V96ZM48,85.34,128,32V208H48ZM112,112v16a8,8,0,0,1-16,0V112a8,8,0,1,1,16,0Zm-32,0v16a8,8,0,0,1-16,0V112a8,8,0,1,1,16,0Zm0,56v16a8,8,0,0,1-16,0V168a8,8,0,0,1,16,0Zm32,0v16a8,8,0,0,1-16,0V168a8,8,0,0,1,16,0Z"
                ></path>
                </svg>
            </div>
            <div class="w-[1.5px] bg-[#d4dbe2] h-2 grow"></div>
            </div>
            <div class="flex flex-1 flex-col py-3">
            <p class="text-[#101418] text-base font-medium leading-normal">Founded Not So Boring Startup</p>
            <p class="text-[#5c738a] text-base font-normal leading-normal">2025</p>
            </div>
            <div class="flex flex-col items-center gap-1">
            <div class="w-[1.5px] bg-[#d4dbe2] h-2"></div>
            <div class="text-[#101418]" data-icon="RocketLaunch" data-size="24px" data-weight="regular">
                <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                <path
                    d="M103.77,185.94C103.38,187.49,93.63,224,40,224a8,8,0,0,1-8-8c0-53.63,36.51-63.38,38.06-63.77a8,8,0,0,1,3.88,15.53c-.9.25-22.42,6.54-25.56,39.86C81.7,204.48,88,183,88.26,182a8,8,0,0,1,15.51,4Zm93-67.4L192,123.31v58.33A15.91,15.91,0,0,1,187.32,193L153,227.3A15.91,15.91,0,0,1,141.7,232a16.11,16.11,0,0,1-5.1-.83,15.94,15.94,0,0,1-10.78-12.92l-5.37-38.49L76.24,135.55l-38.47-5.37A16,16,0,0,1,28.7,103L63,68.68A15.91,15.91,0,0,1,74.36,64h58.33l4.77-4.77c26.68-26.67,58.83-27.82,71.41-27.07a16,16,0,0,1,15,15C224.6,59.71,223.45,91.86,196.78,118.54ZM40,114.34l37.15,5.18L116.69,80H74.36ZM91.32,128,128,164.68l57.45-57.45a76.46,76.46,0,0,0,22.42-59.16,76.65,76.65,0,0,0-59.11,22.47ZM176,139.31l-39.53,39.53L141.67,216,176,181.64Z"
                ></path>
                </svg>
            </div>
            <div class=" bg-[#d4dbe2] h-2 grow"></div>
            </div>
            <div class="flex flex-1 flex-col py-3">
            <p class="text-[#101418] text-base font-medium leading-normal">Launched Our First Application</p>
            <p class="text-[#5c738a] text-base font-normal leading-normal">2025</p>
            </div>
            
        </div>
       
        </div>
    </div>
    </div>
</div>
