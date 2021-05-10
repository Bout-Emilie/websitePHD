<script>
    export let contact_info={};
    const {ADDRESS,DEPARTEMENT,INSTITUTE,WEBSITEDEPARTEMENT,WEBSITEINSTITURE,ADDRESS2} = contact_info;
</script>

<aside class="mt-10 ml-10 space-y-3 flex flex-col">
    <h2 class="font-mono uppercase text-base text-red-800" >Contact</h2>
    <div class="adress text-lg">{ADDRESS}</div>
    <div class="adress text-lg">{ADDRESS2}</div>
    <div class="departement no-underline hover:underline text-red-800 text-lg"> <a href={WEBSITEDEPARTEMENT}>{DEPARTEMENT}</a></div>
    <div class="institue no-underline hover:underline text-red-800 text-lg"> <a href={WEBSITEINSTITURE}>{INSTITUTE}</a></div>
    <div class="email ">emilie.bout@inria.fr</div>
    <div class="logo flex space-x-4 ">
        <div class=""><a href="https://scholar.google.fr/citations?user=K9mjGDUAAAAJ&hl=fr&oi=ao"><img alt='Google Scholar' src='google-plus.png' class="max-width"></a></div>
        <div class=""><a href="https://www.linkedin.com/in/emilie-bout-050a68117/?originalSubdomain=fr"><img alt='Linkedin' src='linkedin.png' class="max-width"></a></div>
        
    </div>
</aside>

<style>
    .max-width {
        max-width: 50px;
    }
</style>