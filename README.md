<h1 align="center">Hi, <img src="https://media4.giphy.com/media/HV0tHmPREaD0sIixmg/giphy.gif?cid=790b7611085cc85000b0bd3d5bbd3e7346d87fdb6155c09b&rid=giphy.gif&ct=g" width="5%" height="5%"/> I'm a Full-stack web developer</h1>
<h3 align="center">Building the future, one line of code at a time !</h3> 

<div class="highlight highlight-source-rust notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">type</span> <span class="pl-smi">Str</span> = <span class="pl-c1">&amp;</span><span class="pl-c1">'</span><span class="pl-ent">static</span> <span class="pl-smi">str</span><span class="pl-kos">;</span>

<span class="pl-c1">#<span class="pl-kos">[</span>derive<span class="pl-kos">(</span><span class="pl-v">Debug</span><span class="pl-kos">)</span><span class="pl-kos">]</span></span>
<span class="pl-k">enum</span> <span class="pl-smi">Principle</span> <span class="pl-kos">{</span> <span class="pl-v">SOLID</span><span class="pl-kos">,</span> <span class="pl-v">DRY</span><span class="pl-kos">,</span> <span class="pl-v">KISS</span><span class="pl-kos">,</span> <span class="pl-v">YAGNI</span><span class="pl-kos">,</span> <span class="pl-v">OPPA_GANGNAM_STYLE</span> <span class="pl-kos">}</span>

<span class="pl-c1">#<span class="pl-kos">[</span>derive<span class="pl-kos">(</span><span class="pl-v">Debug</span><span class="pl-kos">)</span><span class="pl-kos">]</span></span>
<span class="pl-k">struct</span> <span class="pl-smi">Stack</span> <span class="pl-kos">{</span>
    <span class="pl-c1">languages</span><span class="pl-kos">:</span> <span class="pl-smi">Vec</span><span class="pl-kos">&lt;</span><span class="pl-smi">Str</span><span class="pl-kos">&gt;</span><span class="pl-kos">,</span>
    <span class="pl-c1">libs_and_frameworks</span><span class="pl-kos">:</span> <span class="pl-smi">Vec</span><span class="pl-kos">&lt;</span><span class="pl-smi">Str</span><span class="pl-kos">&gt;</span><span class="pl-kos">,</span>
    <span class="pl-c1">devops</span><span class="pl-kos">:</span> <span class="pl-smi">Vec</span><span class="pl-kos">&lt;</span><span class="pl-smi">Str</span><span class="pl-kos">&gt;</span><span class="pl-kos">,</span>
    <span class="pl-c1">databases</span><span class="pl-kos">:</span> <span class="pl-smi">Vec</span><span class="pl-kos">&lt;</span><span class="pl-smi">Str</span><span class="pl-kos">&gt;</span><span class="pl-kos">,</span>
<span class="pl-kos">}</span>

<span class="pl-c1">#<span class="pl-kos">[</span>derive<span class="pl-kos">(</span><span class="pl-v">Debug</span><span class="pl-kos">)</span><span class="pl-kos">]</span></span>
<span class="pl-k">struct</span> <span class="pl-smi">Profile</span> <span class="pl-kos">{</span>
    <span class="pl-c1">name</span><span class="pl-kos">:</span> <span class="pl-smi">Str</span><span class="pl-kos">,</span>
    <span class="pl-c1">from</span><span class="pl-kos">:</span> <span class="pl-smi">Str</span><span class="pl-kos">,</span>
    <span class="pl-c1">current_in</span><span class="pl-kos">:</span> <span class="pl-smi">Str</span><span class="pl-kos">,</span>
    <span class="pl-c1">principles</span><span class="pl-kos">:</span> <span class="pl-smi">Vec</span><span class="pl-kos">&lt;</span><span class="pl-smi">Principle</span><span class="pl-kos">&gt;</span><span class="pl-kos">,</span>
    <span class="pl-c1">tech</span><span class="pl-kos">:</span> <span class="pl-smi">Stack</span><span class="pl-kos">,</span>
<span class="pl-kos">}</span>

<span class="pl-k">fn</span> <span class="pl-en">main</span><span class="pl-kos">(</span><span class="pl-kos">)</span> -&gt; <span class="pl-kos">(</span><span class="pl-kos">)</span> <span class="pl-kos">{</span>

    <span class="pl-k">let</span> profile = <span class="pl-smi">Profile</span> <span class="pl-kos">{</span>
        <span class="pl-c1">name</span><span class="pl-kos">:</span> <span class="pl-s">"Rafael Milewski"</span><span class="pl-kos">,</span>
        <span class="pl-c1">from</span><span class="pl-kos">:</span> <span class="pl-s">"Brazil"</span><span class="pl-kos">,</span>
        <span class="pl-c1">current_in</span><span class="pl-kos">:</span> <span class="pl-s">"China"</span><span class="pl-kos">,</span>
        <span class="pl-c1">principles</span><span class="pl-kos">:</span> <span class="pl-en">vec</span><span class="pl-en">!</span><span class="pl-kos">[</span> <span class="pl-v">Principle</span>::<span class="pl-v">SOLID</span>, <span class="pl-v">Principle</span>::<span class="pl-v">DRY</span>, <span class="pl-v">Principle</span>::<span class="pl-v">YAGNI</span>, <span class="pl-v">Principle</span>::<span class="pl-v">KISS</span> <span class="pl-kos">]</span><span class="pl-kos">,</span>
        <span class="pl-c1">tech</span><span class="pl-kos">:</span> <span class="pl-smi">Stack</span> <span class="pl-kos">{</span>
            <span class="pl-c1">languages</span><span class="pl-kos">:</span> <span class="pl-en">vec</span><span class="pl-en">!</span><span class="pl-kos">[</span> <span class="pl-s">"HTML/CSS"</span>, <span class="pl-s">"Typescript"</span>, <span class="pl-s">"PHP"</span>, <span class="pl-s">"Dart"</span>, <span class="pl-s">"Rust"</span> <span class="pl-kos">]</span><span class="pl-kos">,</span>
            <span class="pl-c1">databases</span><span class="pl-kos">:</span> <span class="pl-en">vec</span><span class="pl-en">!</span><span class="pl-kos">[</span> <span class="pl-s">"Redis"</span>, <span class="pl-s">"MySQL"</span>, <span class="pl-s">"Meilisearch"</span>, <span class="pl-s">"MongoDB"</span>, <span class="pl-s">"SurrealDB"</span> <span class="pl-kos">]</span><span class="pl-kos">,</span>
            <span class="pl-c1">libs_and_frameworks</span><span class="pl-kos">:</span> <span class="pl-en">vec</span><span class="pl-en">!</span><span class="pl-kos">[</span>
                <span class="pl-s">"Vue.js"</span>, <span class="pl-s">"React"</span>, <span class="pl-s">"Svelte"</span>,
                <span class="pl-s">"Webpack"</span>, <span class="pl-s">"Vite"</span>, <span class="pl-s">"Tailwind"</span>, <span class="pl-s">"SASS"</span>,
                <span class="pl-s">"Three.js"</span>, <span class="pl-s">"Pixi.js"</span>,
                <span class="pl-s">"Nuxt"</span>, <span class="pl-s">"Next"</span>, <span class="pl-s">"Nodejs"</span>,
                <span class="pl-s">"Flutter"</span>, <span class="pl-s">"NativeScript"</span>,
                <span class="pl-s">"Laravel"</span>, <span class="pl-s">"Nova"</span>, <span class="pl-s">"GraphQL"</span>,
            <span class="pl-kos">]</span><span class="pl-kos">,</span>
            <span class="pl-c1">devops</span><span class="pl-kos">:</span> <span class="pl-en">vec</span><span class="pl-en">!</span><span class="pl-kos">[</span>
                <span class="pl-s">"Linux"</span>, <span class="pl-s">"Docker + Swarm"</span>, <span class="pl-s">"Caddy"</span>, <span class="pl-s">"Traefik"</span>, <span class="pl-s">"Terraform"</span>,
                <span class="pl-s">"CD/CI (Github Actions, Dagger, Drone)"</span>,
                <span class="pl-s">"Monitoring (TICK Stack)"</span>,
                <span class="pl-s">"Cloud Hosting (Alibaba Cloud, GCP, AWS, Vultr, DO)"</span>,
            <span class="pl-kos">]</span><span class="pl-kos">,</span>
        <span class="pl-kos">}</span><span class="pl-kos">,</span>
    <span class="pl-kos">}</span><span class="pl-kos">;</span>

    <span class="pl-en">println</span><span class="pl-en">!</span><span class="pl-kos">(</span><span class="pl-s">"Hi, thanks for checking out my {:#?}"</span>, profile<span class="pl-kos">)</span><span class="pl-kos">;</span>

<span class="pl-kos">}</span></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="type Str = &amp;'static str;

#[derive(Debug)]
enum Principle { SOLID, DRY, KISS, YAGNI, OPPA_GANGNAM_STYLE }

#[derive(Debug)]
struct Stack {
    languages: Vec<Str>,
    libs_and_frameworks: Vec<Str>,
    devops: Vec<Str>,
    databases: Vec<Str>,
}

#[derive(Debug)]
struct Profile {
    name: Str,
    from: Str,
    current_in: Str,
    principles: Vec<Principle>,
    tech: Stack,
}

fn main() -> () {

    let profile = Profile {
        name: &quot;Rafael Milewski&quot;,
        from: &quot;Brazil&quot;,
        current_in: &quot;China&quot;,
        principles: vec![ Principle::SOLID, Principle::DRY, Principle::YAGNI, Principle::KISS ],
        tech: Stack {
            languages: vec![ &quot;HTML/CSS&quot;, &quot;Typescript&quot;, &quot;PHP&quot;, &quot;Dart&quot;, &quot;Rust&quot; ],
            databases: vec![ &quot;Redis&quot;, &quot;MySQL&quot;, &quot;Meilisearch&quot;, &quot;MongoDB&quot;, &quot;SurrealDB&quot; ],
            libs_and_frameworks: vec![
                &quot;Vue.js&quot;, &quot;React&quot;, &quot;Svelte&quot;,
                &quot;Webpack&quot;, &quot;Vite&quot;, &quot;Tailwind&quot;, &quot;SASS&quot;,
                &quot;Three.js&quot;, &quot;Pixi.js&quot;,
                &quot;Nuxt&quot;, &quot;Next&quot;, &quot;Nodejs&quot;,
                &quot;Flutter&quot;, &quot;NativeScript&quot;,
                &quot;Laravel&quot;, &quot;Nova&quot;, &quot;GraphQL&quot;,
            ],
            devops: vec![
                &quot;Linux&quot;, &quot;Docker + Swarm&quot;, &quot;Caddy&quot;, &quot;Traefik&quot;, &quot;Terraform&quot;,
                &quot;CD/CI (Github Actions, Dagger, Drone)&quot;,
                &quot;Monitoring (TICK Stack)&quot;,
                &quot;Cloud Hosting (Alibaba Cloud, GCP, AWS, Vultr, DO)&quot;,
            ],
        },
    };

    println!(&quot;Hi, thanks for checking out my {:#?}&quot;, profile);

}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success m-2 d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>

- <img src="https://media3.giphy.com/media/H59XwE8tzGm6k6BN98/giphy.gif?cid=790b7611bb0ce0ec7171672d9d6a40a0be1933ce54eb0bcf&rid=giphy.gif&ct=s" height="2%" width="2%"/> I’m currently working **@Zuse Technologies**

- 🌱 An enthusiast in learning frameworks like Laravel, NextJs, Angular and more.

-  Yo : **It's not a bug,<img src="https://media1.giphy.com/media/K0XHQRUgkpRlRmkvll/giphy.gif?cid=790b7611e3fb9fadfc44059e3281435b2ea2553d73baddbc&rid=giphy.gif&ct=s" height="3%" width="3%"/> it's an undocumented feature!**

- Connect with me **sandev.net@gmail.com** <img src="https://github.com/TheDudeThatCode/TheDudeThatCode/raw/master/Assets/Handshake.gif" width="5%" height="5%"/>

[![trophy](https://github-profile-trophy.vercel.app/?username=sandevD&theme=onestar&row=2&column=3)](https://github.com/ryo-ma/github-profile-trophy)

<p align="center">
</p>

<h3 align="center">Languages and Tools:</h3>
<p align="left"> <a href="https://angular.io" target="_blank" rel="noreferrer"> <img src="https://angular.io/assets/images/logos/angular/angular.svg" alt="angular" width="40" height="40"/> </a> <a href="https://angular.io" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original-wordmark.svg" alt="angularjs" width="40" height="40"/> </a> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"/> </a> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://laravel.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/laravel/laravel-plain-wordmark.svg" alt="laravel" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://nextjs.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/nextjs-2.svg" alt="nextjs" width="40" height="40"/> </a> <a href="https://www.photoshop.com/en" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/photoshop/photoshop-line.svg" alt="photoshop" width="40" height="40"/> </a> <a href="https://www.php.net" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="40" height="40"/> </a> </p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=sandevD&show_icons=true&locale=en&theme=cobalt" alt="sandevd" /></p>

<p><a href="https://git.io/streak-stats"><img src="https://github-readme-streak-stats.herokuapp.com?user=sandevD&theme=cobalt&hide_border=false&border_radius=4.5&locale=en&date_format=&mode=daily&exclude_days=&sections=total%2Ccurrent%2Clongest&card_width=495&type=svg&background-type=solid&properties=background" alt="GitHub Streak" /></a></p>

