<script>
import { base } from "$app/paths";
import radauLogo from "$lib/images/radau-logo.svg";
</script>

<svelte:head>
    <title>Radau</title>
    <meta name="description" content="Radau Homepage" />
</svelte:head>
<section class="flex flex-col items-center justify-center">
    <img src={radauLogo} alt="Radau Logo" class="h-96" />

    <p class="py-10 text-3xl">
        Welcome to RAD.AU your friendly neighbourhood bicycle workshop
        collective.
    </p>
    <p>
        We are open <span class="font-bold">every Sunday</span> from
        <span class="font-bold">14:00 to 17:00</span>
        for the public. Our concept is simple: we have the tools, you have the hands,
        and if you need help, we will try our best. We also have a collection of
        new and used parts. Everything works over donations, so please give as much
        as possible for you.
        <br /> <br />

        We are also known for organising cycling events and concerts. Head over
        to our <a href="{base}/events">events page</a> or our
        <a href="https://www.instagram.com/rad_au/" target="_blank"
            >instagram page</a
        > to see what's coming up!
    </p>
    <iframe
        title="Radau on the map"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2863.89871199123!2d7.409212360469519!3d46.9447528855772!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x478e3905c0645b2d%3A0x43f2b1d7b4f20288!2sFreiburgstrasse%20121%2C%203008%20Bern!5e0!3m2!1sen!2sch!4v1716560496102!5m2!1sen!2sch"
        class="h-80 w-80 py-5"
        style="border:0;"
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
    ></iframe>
</section>
