<template>
    <header>
        <h1 
        class="flex items-center my-auto text-2xl text-white h-24 py-3 px-5 
        bg-gradient-to-r from-cyan-500 to-indigo-500 shadow shadow-lg">客戶網站語系維護
        </h1>
    </header>

    <nav>
        
    </nav>


    <div class="right container mx-auto flex justify-end items-center mt-4">
        <div class="updateTime mr-4">資料庫最後更新時間：<span class="timeing">2023-02-02 11:35:25</span> </div>
        <div class="btnGroup">
            <button class="mr-2 btn-blue">匯出</button>
            <button class="btn-blue">匯入</button>
        </div>
    </div>
    
<div class="mb-4 border-b border-gray-200 dark:border-gray-700">
    <ul class="flex flex-wrap -mb-px text-sm font-medium text-center" id="Tab" data-tabs-toggle="#TabContent" role="tablist">
        <li class="mr-2" role="presentation">
            <button class="inline-block p-4 border-b-2 rounded-t-lg" id="languageList-tab" data-tabs-target="#languageList" type="button" role="tab" aria-controls="profile" aria-selected="false">語言列表</button>
        </li>
        <li class="mr-2" role="presentation">
            <button class="inline-block p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-indigo-500 dark:hover:text-gray-300" id="batchImport-tab" data-tabs-target="#batchImport" type="button" role="tab" aria-controls="dashboard" aria-selected="false">批次匯入</button>
        </li>
    </ul>
</div>
<div id="TabContent">
    <div class=" p-4 rounded-lg bg-gray-50 dark:bg-gray-800" id="languageList" role="tabpanel" aria-labelledby="languageList-tab">
        <p class="text-sm text-gray-500 dark:text-gray-400">This is some placeholder content the <strong class="font-medium text-gray-800 dark:text-white">Profile tab's associated content</strong>. Clicking another tab will toggle the visibility of this one for the next. The tab JavaScript swaps classes to control the content visibility and styling.</p>
    </div>
    <div class=" p-4 rounded-lg bg-gray-50 dark:bg-gray-800" id="batchImport" role="tabpanel" aria-labelledby="batchImport-tab">
        <p class="text-sm text-gray-500 dark:text-gray-400">This is some placeholder content the <strong class="font-medium text-gray-800 dark:text-white">Dashboard tab's associated content</strong>. Clicking another tab will toggle the visibility of this one for the next. The tab JavaScript swaps classes to control the content visibility and styling.</p>
    </div>
</div>

    <div class="example container mx-auto mt-8">
        <p>範例：</p>
            <ul class="content-area py-2 px-4">
                <li class="text-red-600">[</li>
                <li class="text-red-600">["key","簡體中文","英文","泰文","越南文"],</li>
                <li class="text-red-600">["key2","簡體中文","法文","西班牙文","日文"]</li>
                <li class="text-red-600">]</li>
            </ul>
            <p class="text-red-700 mt-4">**這裡不會擋重複的Key，請放心</p>
    </div> 

</template>
<script setup lang="ts">


</script>
