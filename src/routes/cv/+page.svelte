<script>
	const updated = 'November 2026';
</script>

<svelte:head>
	<title>Euan Ripper — CV</title>
</svelte:head>

<main class="cv">
	<header class="head">
		<h1>Euan Ripper</h1>
		<p class="tagline">Engineer · Programme Lead &amp; Web Developer @ Hack Club</p>
		<p class="contact">
			<a href="mailto:euan@hackclub.com">euan@hackclub.com</a>
		</p>
	</header>

	<section>
		<p class="summary">
			Robotics and mechatronics student at Loughborough, currently working as a web developer
			and event organiser for Hack Club. I build platforms and run programmes that have rewarded
			thousands of teenagers for learning technical skills. I grew up on a sustainable farm in
			rural Devon and care most about energy resilience and sustainability.
		</p>
	</section>

	<section>
		<h2>Experience</h2>

		<article class="role">
			<div class="role-head">
				<h3>Hack Club — Programme Lead &amp; Web Developer</h3>
				<span class="meta">United States · 2024 – present</span>
			</div>
			<ul>
				<li>Selected onto a $50,000 fellowship after two interviews and a portfolio review; one of a small hand-picked group running Hack Club's funding programmes from its US headquarters. Deferred a place at Loughborough to take it.</li>
				<li>Led communications for Summer of Making, a global programme run with GitHub that shipped over 5,000 physical prizes to teenagers who built technical projects.</li>
				<li>Designed and built Beest, a full-stack web platform, from scratch: more than 4,000 verified students built projects, received feedback and earned physical prizes. Modelled a Strandbeest linkage in CAD and flew the top 30 builders to the Netherlands to build Strandbeests and meet Theo Jansen. One of Hack Club's first events in Europe; Net Promoter Score of 94.</li>
				<li>Co-created a Los Angeles hackathon with the Open Sauce team, Michael Reeves, William Osman and eight other YouTubers (combined audience around 25 million).</li>
				<li>Ran programmes that generated over 10,000 hours of independently verified student work; managed $100k+ budgets, logistics, event safety and deadlines to thousands of users.</li>
				<li>Handled a responsible security disclosure end to end: after a researcher reported a bug exposing user emails on a platform I oversaw, I confirmed it, took the platform offline, patched it and rewarded the reporter. I then searched the logs for the exposure window, emailed all 25 possibly affected users, scheduled training for the developer and open-sourced the platform.</li>
			</ul>
		</article>

		<article class="role">
			<div class="role-head">
				<h3>North Devon Robotics Club — Founder &amp; Team Lead</h3>
				<span class="meta">Devon · from age 16</span>
			</div>
			<ul>
				<li>Taught myself the engineering, then taught my members, growing the club from zero to 15 regular participants.</li>
				<li>Led the team to win the North Devon Robotics Challenge 2024 against far better-funded private schools. Credited as team lead in an <a href="https://engx.theiet.org/b/blogs/posts/north-devon-robotics-challenge-2024">IET article</a>.</li>
			</ul>
		</article>
	</section>

	<section>
		<h2>Education</h2>
		<article class="role">
			<div class="role-head">
				<h3>Loughborough University</h3>
				<span class="meta">Mechatronics, robotics &amp; control engineering</span>
			</div>
		</article>
		<article class="role">
			<div class="role-head">
				<h3>A-Levels</h3>
				<span class="meta">perfect score in programming</span>
			</div>
		</article>
	</section>

	<section>
		<h2>Leadership &amp; teamwork</h2>
		<article class="role">
			<div class="role-head">
				<h3>Ten Tors 2025 — Team Leader</h3>
				<span class="meta">Dartmoor · May 2025</span>
			</div>
			<ul>
				<li>Led a team of six from QE School Crediton through the 55-mile endurance challenge, completing it in 33 hours despite record dropouts from heat stroke. Each member carried around 20kg to be self-sufficient for the weekend.</li>
			</ul>
		</article>
	</section>

	<section>
		<h2>Interests</h2>
		<ul>
			<li>Challenge-driven hobbies: unicycling (started at 16), ultramarathons (first 50k finished in eight hours, at 17), and learning to rollerblade at 19.</li>
			<li>Building in my spare time: designed and built my own walking Strandbeest, and I'm currently hacking a cheap thermal printer to print live photos from a Pi Camera.</li>
		</ul>
	</section>

	<footer class="foot">
		<a href="/">← back to euanripper</a>
		<span class="updated">updated {updated}</span>
	</footer>
</main>

<style>
	.cv {
		max-width: 820px;
		margin: 0 auto;
		padding: 3rem 1.5rem 4rem;
		line-height: 1.55;
	}

	.head {
		margin-bottom: 2.5rem;
	}

	h1 {
		font-size: 2.5rem;
		margin: 0;
	}

	.tagline {
		font-size: 1.1rem;
		margin: 0.4rem 0 0;
		color: #555;
	}

	.contact {
		margin: 0.6rem 0 0;
		font-size: 1rem;
	}

	a {
		color: #2563eb;
	}

	.summary {
		font-size: 1.1rem;
		margin: 0;
	}

	section {
		margin-top: 2.25rem;
	}

	h2 {
		font-size: 1.1rem;
		text-transform: uppercase;
		letter-spacing: 0.08em;
		border-left: 4px solid #ec3750;
		padding-left: 0.6rem;
		margin: 0 0 1rem;
	}

	.role {
		margin-bottom: 1.5rem;
	}

	.role-head {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		align-items: baseline;
		gap: 0.25rem 1rem;
	}

	h3 {
		font-size: 1.05rem;
		margin: 0;
	}

	.meta {
		color: #777;
		font-size: 0.9rem;
	}

	ul {
		margin: 0.5rem 0 0;
		padding-left: 1.1rem;
	}

	li {
		margin-bottom: 0.4rem;
	}

	.foot {
		margin-top: 3rem;
		padding-top: 1rem;
		border-top: 1px solid #ccc;
		display: flex;
		justify-content: space-between;
		font-size: 0.9rem;
		color: #777;
	}

	.foot a {
		text-decoration: none;
	}

	@media print {
		a {
			color: #000;
		}
		.foot {
			display: none;
		}
		.cv {
			padding: 0;
		}
	}
</style>
