<script lang="ts">
	import DaisyUiAvatar from "../library/daisyui/avatar/DaisyUiAvatar.svelte";
import DaisyUiButton from "../library/daisyui/button/DaisyUiButton.svelte";
	import DaisyUiDropdown from "../library/daisyui/dropdown/DaisyUiDropdown.svelte";
	import DaisyUiMenu from "../library/daisyui/menu/DaisyUiMenu.svelte";
	import DaisyUiNavbarCenter from "../library/daisyui/navbar/center/DaisyUiNavbarCenter.svelte";
	import DaisyUiNavbar from "../library/daisyui/navbar/DaisyUiNavbar.svelte";
	import DaisyUiNavbarEnd from "../library/daisyui/navbar/end/DaisyUiNavbarEnd.svelte";
	import DaisyUiNavbarStart from "../library/daisyui/navbar/start/DaisyUiNavbarStart.svelte";



</script>


<div class="absolute top-0 left-0 right-0">
<DaisyUiNavbar className=" bg-base-100 shadow-sm mx-auto ">

    

    <DaisyUiNavbarStart >
        <DaisyUiDropdown className="d-dropdown">

            
          
                <div class="d-drawer">
  <input id="my-drawer" type="checkbox" class="d-drawer-toggle" />
  <div class="d-drawer-content">
    <!-- Page content here -->
    <label for="my-drawer" class="d-btn-ghost d-btn-circle"><svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"> <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h7" /> </svg> </label>
  </div>
  <div class="d-drawer-side">
    <label for="my-drawer" aria-label="close sidebar" class="d-drawer-overlay"></label>
    <DaisyUiMenu className="bg-base-200 text-base-content min-h-full w-80 p-5 pt-8 pl-23">
      
        <DaisyUiAvatar className="d-avatar-placeholder absolute left-10 top-9">
            <div class="bg-neutral text-neutral-content w-10 rounded-full">
    

        </DaisyUiAvatar>
      <p class="text-md">Mari2020</p>
      <p>Mari2020@gmail.com</p>

      <DaisyUiButton className="bg-gray-700 text-white rounded text-xs  absolute left-10 top-25 " onClick={() => console.log("Hello")}>Change Account</DaisyUiButton>

      <div class="mt-36  absolute left-10 text-xs "> 
      <h1 class="text-lg  mb-4">All Pages</h1> 

      <div class="leading-5">
     <li><a href="">Pages 1</a></li>
     <li><a href="">Pages 2</a></li>
     <li><a href="">Pages 3</a></li>
     </div>

     <h1 class="text-lg mt-9  mb-4">Categories</h1> 
     
     <div class="leading-5">
     <li><a href="">Category 1</a></li>
     <li><a href="">Category 2</a></li>
     <li><a href="">Category 3</a></li>
     </div>

     <h1 class="text-lg mt-9 mb-4">Help & Support</h1> 

     <div class="leading-5">
     <li><a href="">Contact Us</a></li>
     <li><a href="">FAQ</a></li>
      </div>
     

     </div>

     

     

      </DaisyUiMenu>
      

     
    
      
        
     


      
  </div>
</div>
      
        
            </DaisyUiDropdown>
         
    </DaisyUiNavbarStart>

    <DaisyUiNavbarCenter>
         <a class="d-btn d-btn-ghost text-xl"><img src="../asset/image/webp/MariLogo.webp"  ></a>
    </DaisyUiNavbarCenter>

    <DaisyUiNavbarEnd>
        <DaisyUiButton className="d-btn-ghost d-btn-circle" onClick={() => console.log("Hello")}>

            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"> <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" /> </svg>
        </DaisyUiButton>

        <DaisyUiButton className="d-btn-ghost d-btn-circle" onClick={() => console.log("Hello")}>
            <div class="d-indicator">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"> <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9" /> </svg>
        <span class="d-badge d-badge-xs d-badge-primary d-indicator-item"></span>
      </div>

        </DaisyUiButton>
    </DaisyUiNavbarEnd>

   

</DaisyUiNavbar>

</div>




	
