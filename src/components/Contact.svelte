<script>
    export let contact_info={};
    const {ADDRESS,DEPARTEMENT,INSTITUTE,WEBSITEDEPARTEMENT,WEBSITEINSTITURE,ADDRESS2} = contact_info;
</script>

<div class="mt-10 ml-10 space-y-3">
    <h2 class="font-mono uppercase text-base text-red-800" >Contact</h2>
    <div class="adress text-lg">{ADDRESS}</div>
    <div class="adress text-lg">{ADDRESS2}</div>
    <div class="departement no-underline hover:underline text-red-800 text-lg"> <a href={WEBSITEDEPARTEMENT}>{DEPARTEMENT}</a></div>
    <div class="institue no-underline hover:underline text-red-800 text-lg"> <a href={WEBSITEINSTITURE}>{INSTITUTE}</a></div>
    <div class="email ">emilie.bout@inria.fr</div>
    <div class="logo flex space-x-4 ">
        <div class="w-1/5"><a href="https://scholar.google.fr/citations?user=K9mjGDUAAAAJ&hl=fr&oi=ao"><img alt='Google Scholar' src='google.png' class=""></a></div>
        <div class="w-1/6 mt-1"><a href="https://www.linkedin.com/in/emilie-bout-050a68117/?originalSubdomain=fr"><img alt='Linkedin' src='linkedin.png' class=""></a></div>
        
    </div>
</div>