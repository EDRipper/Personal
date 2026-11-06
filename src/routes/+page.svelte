<script>
  import { preloadData } from '$app/navigation';
    import { cubicOut } from 'svelte/easing';
    import { tweened } from 'svelte/motion';

    export let target = 10000;
    
    const count = tweened(0, {
        duration: 5000,
        easing: cubicOut
    });

    $: count.set(target);
</script>

<div class="wrapper">
<main class="page">
    <h1>Hi! I'm Euan Ripper, Engineer <a href="https://hackclub.com" class="hackclub">@Hack Club</a></h1>
    <p>
        I learnt to code to <a href="#boringJob">automate a very boring job</a>, and it ended up landing me a dream job!
        At Hack Club I organise events and create platforms that reward teenagers for learning new skills.<br><br>
        Directly through my programs, teens have tracked <b>{$count.toFixed(0)} hours</b> building new skills.
    </p>
    <br><br>
    <div class="card-grid">
        
        <article class="card">  
            <img src="/src/lib/assets/summer-of-making.png" class="card-image">
            <footer class="card-footer">
                <h3>Summer Of Making</h3>
                Virtual coding challenge, build any project, get a prize. <br> I worked on:
                <ul>
                    <li>-improving user funnel</li>
                    <li>-communications and outreach</li>
                </ul>
            </footer>
        </article>
    
        <article class="card">  
            <img src="https://midnight.hackclub.com/logo.svg" class="card-image">
            <footer class="card-footer">
                <h3>Midnight Hackathon</h3>
                X person murder mystery Hackathon in Vienna,  <br   ><br> I worked on: 
                <ul>
                    <li>-improving user funnel</li>
                    <li>-communications and outreach</li>
                </ul>
            </footer>
        </article>
        <a href="summer.hackclub.com" class="card">  
            <img src="/src/lib/assets/emerge.png" class="card-image">
            <footer class="card-footer">
                <h3>Emerge Challenge</h3>
                    Develop an emergent behaviour, contribute to an emerging picture. <br><br> I worked on:
                <ul>
                    <li>-improving user funnel</li>
                    <li>-communications and outreach</li>
                </ul>
            </footer>
        </a>
        <article class="card">  
            <img src="/src/lib/assets/summer-of-making.png" class="card-image">
            <footer class="card-footer">
                <h3>Grand Expedition</h3>
                Virtual coding challenge, build any project, get a prize. <br> I worked on:
                <ul>
                    <li>-improving user funnel</li>
                    <li>-communications and outreach</li>
                </ul>
            </footer>
        </article>
        <article class="card">  
            <img src="/src/lib/assets/summer-of-making.png" class="card-image">
            <footer class="card-footer">
                <h3>Flagship Hackathon</h3>
                Virtual coding challenge, build any project, get a prize. <br> I worked on:
                <ul>
                    <li>-improving user funnel</li>
                    <li>-communications and outreach</li>
                </ul>
            </footer>
        </article>
        <article class="card">  
            <img src="/src/lib/assets/summer-of-making.png" class="card-image">
            <footer class="card-footer">
                <h3>HC Dummies</h3>
                Virtual coding challenge, Learn a new language, get rewards. <br> I worked on:
                <ul>
                    <li>-improving user funnel</li>
                    <li>-communications and outreach</li>
                </ul>
            </footer>
        </article>
    </div>

    <div class="banner">
        <a class="banner-text">Get My Resume  </a>
        <a class="banner-text" href="/cv">  Get My CV  </a>
        <a class="banner-text">  Get My Qualifications  </a>
        <a class="banner-text">  See My Personal Work  </a>
    </div>
    </main>
</div>
<div class="triangle">
    <!--big 3d triangle-->
</div>
<p class="outside-work">
    outside of work I like using code to visualise maths.
</p>


<div class="text-content">
<h2>My story:   </h2>
<p id="boringJob"> At 16 I lived in rural england, working minimum wage at the nearest agricultural warehouse. There I would find stock photos online, square them, remove the background and upload them to the warehouse's new website. After nearly developing RSI I worked out that this kind of labourious work would be much better suited to automations, so I sat down and worked out my first python script. <br>It worked pretty well, but i never had the courage to explain my sudden increase in productivity.<br><br>
I loved being able to do monotonous things with code, but i pretty quickly worked out I could also do creative things. I started using code as a tool to explore problems in maths and science, generating 3d models of mathematical fractals to print out, and writing simulations to visualise differential equations i was learning in maths class. I wanted to share how great programming was with everyone, but in my tiny school only 5 people studied A-Level computer science, and it wasn't even taught to the younger years in the school.<br><br> I couldn't stand for that, so in my school lunch break I would hike up the hill to the younger years campus where I would coach the kids through everything I taught myself about coding and building. I even reached out to a competition organiser, we technically weren't in the elegible area for the competition, but there were 0 other competitions available. I secured funding, made announcements and coached a team to come to the <a href="fill in later">North Devon Robotics Competetion.</a> <br><br> After 6 weeks of coaching we showed up as the team with the least funding, and the only team new to the event. Despite that the team owned the competition with both winning on overall points and winning the design award, for which they recieved recognition at the <a href="fill in later">North Devon Annual Awards Ceremony.</a> I used the prize money to continue running a coding club available to all years, which is when I found out about <a hred="https://hackclub.com">Hack Club</a>, an American non-profit providing coding workshops, tools and advice for club leaders.
<br><br>
After running a Hack Club for a full year I graduated out of high school with a perfect score in programming, ready to move on to university. That was when I got an email from Hack Club, an open invitation to apply for a gap year position. I filled out the form hoping to get interview practice before Uni, with no real expectation of it going anywhere, especially since Hack Club was in the USA and I was stuck in drousy England. They checked out my portfolio, interveiwed me (Twice) and then offered me a job and a plane ticket to Vermont!
</div>
    


<footer>
    <p><a href="mailto:euan@hackclub.com">euan@hackclub.com</a></p>
</footer>
<style>
    .page {
        padding: 2rem 2rem 2rem;
    }

    .hackclub {
        color: #eee;
        font-family: 'Phantom Sans', sans-serif;
        border-radius: 10px;
        padding: 8px 16px;
        display: inline-block;
        background-color: #ec3750;
    }

    h1 {
        font-size: 2.5rem;
    }

    p {
        font-size: 1.25rem;
    }

    b {
        color: #ec3750;
    }


    a {
        color: #2563eb;
    }

    .wrapper {
        min-height: 100vh;
        display: flex;
        flex-direction: column;
    }
    .page {
        flex: 1;
    }
    
    footer {
        background-color: black;
        color: white;
        text-align: center;
        padding: 1rem 0;
    }
    footer a {
        text-decoration: none;
        color: inherit;
    }

 

    @font-face {
        font-family: 'Phantom Sans';
        src: url('https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Bold.woff') format('woff'),
            url('https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Bold.woff2') format('woff2');
        font-weight: bold;
        font-style: normal;
        font-display: swap;
    }
    
    .outside-work {
        display: inline-block;
        color: blue;
        
        transform: rotate(63deg) translate(-19vw, 0vw);
    }
    .triangle{
        width: 0;
        height: 0;
        border-left: 0px solid transparent;
        border-right: 15vw solid transparent;
        border-bottom: 30vw solid #ff0000;
    }
    
    .text-content{
        padding: 2vw;
    }

    .card-grid{
        display: grid;
        gap: 2rem;
        align-items: center;
        padding: 2rem;
        grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    }

    .card{
        display: block;
        border: 1px solid #000;
        border-radius: 8px;
        padding: 1.55rem;
        background: white;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }

    .card-grid a.card {
        color: inherit;
        text-decoration: none;
    }

    .card-image{
        width: 100%;
        height: 100%;
        object-fit: auto;}
    
    .card-footer {
        padding: 1rem;
        border-top: 1px solid #eee;
        margin-top: auto;
        background: none;
        color: inherit;
        text-align: left;
        font-size: smaller;
    }

    .banner {
    padding: 1rem;
    background-color: #000000;
    color: #fff !important; 
    

    }

    .banner-text {
        padding-left: 6vw;
        padding-right: 6vw;
        color: inherit;
        text-align: center;
        

    }
</style>
