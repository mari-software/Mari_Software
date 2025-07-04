<script lang="ts">
	import DaisyUiButton from "$lib/component/library/daisyui/button/DaisyUiButton.svelte";
	import DaisyUiCardBodyAction from "$lib/component/library/daisyui/card/body/action/DaisyUiCardBodyAction.svelte";
	import DaisyUiCardBody from "$lib/component/library/daisyui/card/body/DaisyUiCardBody.svelte";
	import DaisyUiCardBodyTitle from "$lib/component/library/daisyui/card/body/title/DaisyUiCardBodyTitle.svelte";
	import DaisyUiCard from "$lib/component/library/daisyui/card/DaisyUiCard.svelte";
	import DaisyUiInputField from "$lib/component/library/daisyui/inputfield/DaisyUiInputField.svelte";


</script>





<DaisyUiCard className=" d-card-side bg-base-100 shadow-sm bg-indigo-200 rounded-md mt-25  ">
    

  <DaisyUiCardBody >
    <DaisyUiCardBodyTitle >
        <h2 class="text-xs font-bold mt-3"><a class="text-blue-600">MARI</a> has whatever you <br/> need</h2>
        <DaisyUiCardBodyAction className="d-card-actions ">
        <DaisyUiButton className="bg-blue-600 text-white w-22 h-8 text-xs absolute bottom-12 left-5 rounded border-none" onClick={() => console.log("Hello")}> See more</DaisyUiButton>
        </DaisyUiCardBodyAction>
    </DaisyUiCardBodyTitle>
  </DaisyUiCardBody>
  <figure>
    <img
      src="../svg/image.png"
      alt="" class="h-40 w-20 mb-1" />
  </figure>

</DaisyUiCard>


<DaisyUiCard className=" d-card-side bg-base-100 shadow-sm bg-indigo-200 rounded-md mt-6 h-30 ">
    
    
  <DaisyUiCardBody >
    <h2 class="absolute top-0 left-0 text-xs bg-blue-600 w-23 rounded-md pl-4 pt-1 h-6 text-white"> Highlight 1</h2>
    <DaisyUiCardBodyTitle >
        
        <h2 class="text-xs  mt-6"> <a class="font-bold "> Product_Name</a> <br/> <a class="text-[9px]">This is description</a> </h2>
        
    </DaisyUiCardBodyTitle>
  </DaisyUiCardBody>
  <figure>
    <img
      src="../svg/image.png"
      alt="" class="h-40 w-20 mb-1" />
  </figure>

</DaisyUiCard>

<h1 class="flex justify-center mt-6 text-[13px] font-bold"> What would you like to search? </h1>

<label class="d-input mt-2 k border-2 rounded-md h-7">
  
  <input type="search" class="text-[11px]" placeholder="Press here to start typing..." />

  <svg class="h-[1em] opacity-50" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
    <g
      stroke-linejoin="round"
      stroke-linecap="round"
      stroke-width="2.5"
      fill="none"
      stroke="currentColor"
    >
      <circle cx="11" cy="11" r="8"></circle>
      <path d="m21 21-4.3-4.3"></path>
    </g>
  </svg>
</label>

<h1 class="flex justify-start mt-6 text-[15px] font-bold"> Product Line-1 </h1>


<div class="flex flex-row gap-3 mb-5 mt-5">
<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

</div>

<div class="flex flex-row gap-3 ">
<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

</div>

<DaisyUiButton className="flex justify-center items-center  bg-blue-600 text-white w-22 h-8 text-xs  rounded border-none ml-24 mt-5" onClick={() => console.log("Hello")}>
    See more
</DaisyUiButton>

<h1 class="flex justify-start mt-8 text-[15px] font-bold"> Product Line-2 </h1>


<div class="flex flex-row gap-3 mb-5 mt-5">
<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

</div>

<div class="flex flex-row gap-3">
<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

</div>

<DaisyUiButton className="flex justify-center items-center  bg-blue-600 text-white w-22 h-8 text-xs  rounded border-none ml-24 mt-5" onClick={() => console.log("Hello")}>
    See more
</DaisyUiButton>

<h1 class="flex justify-start mt-8 text-[15px] font-bold"> Product Line-3 </h1>


<div class="flex flex-row gap-3 mb-5 mt-5">
<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

</div>

<div class="flex flex-row gap-3">
<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[95px] shadow-sm rounded bg-indigo-200 ">
    <figure>
    <img
      src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
      alt="Shoes" class="w-16 justify-start mt-2 absolute left-2 top-0 "/>
        </figure>

    <DaisyUiCardBody >
        <DaisyUiCardBodyTitle className="text-xs absolute left-2 top-14 font-bold">
            <h2>Product Name</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-2 top-18">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

</div>

<DaisyUiButton className="flex justify-center items-center  bg-blue-600 text-white w-22 h-8 text-xs  rounded border-none ml-24 mt-5" onClick={() => console.log("Hello")}>
    See more
</DaisyUiButton>

<h1 class="flex justify-start mt-8 text-[15px] font-bold"> Articles</h1>


<div class="flex flex-row gap-3 mb-4 mt-5">
<DaisyUiCard className="bg-base-100 w-[150px] h-[92px] shadow-sm rounded bg-indigo-200 ">
    

    <DaisyUiCardBody className="mt-1">
        <DaisyUiCardBodyTitle className="text-xs  font-bold absolute left-4">
            <h2>Article-1</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-4 top-12">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[92px] shadow-sm rounded bg-indigo-200 ">
    

    <DaisyUiCardBody className="mt-1">
        <DaisyUiCardBodyTitle className="text-xs  font-bold absolute left-4">
            <h2>Article-1</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-4 top-12">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>


</div>

<div class="flex flex-row gap-3 mb-4 mt-5">
<DaisyUiCard className="bg-base-100 w-[150px] h-[92px] shadow-sm rounded bg-indigo-200 ">
    

    <DaisyUiCardBody className="mt-1">
        <DaisyUiCardBodyTitle className="text-xs  font-bold absolute left-4">
            <h2>Article-1</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-4 top-12">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>

<DaisyUiCard className="bg-base-100 w-[150px] h-[92px] shadow-sm rounded bg-indigo-200 ">
    

    <DaisyUiCardBody className="mt-1">
        <DaisyUiCardBodyTitle className="text-xs  font-bold absolute left-4">
            <h2>Article-1</h2>
           
        </DaisyUiCardBodyTitle >
         <p class="text-[9px] absolute left-4 top-12">This is description</p>
    </DaisyUiCardBody>

</DaisyUiCard>


</div>



<DaisyUiButton className="flex justify-center items-center  bg-blue-600 text-white w-22 h-8 text-xs  rounded border-none ml-24 mt-5 mb-4" onClick={() => console.log("Hello")}>
    See more
</DaisyUiButton>