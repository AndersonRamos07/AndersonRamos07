```
class Profile{
  constructor()
};
const in_github = new Profile();
/* ----- Contact info ----- */
  in_github.author-name = 'Anderson Ramos',
  in_github.email = 'andersonramos07@live.com';
  in_github.networking = 'in/anderson-ramos07';
/* ----- ----- ----- ----- */
  in_github.repositories = 28;
  in_github.technologies= [
    api-tools: [ 'browser-devtools', 'insomnia', 'postman' ],
    container-platforms: [ 'docker', 'kubernetes_k8s' ],
    cloud: 'oracle-cloud-instrastructure_oci',
    ides: [ 'intellij', 'vs-code', 'eclipse' , 'android-studio' ],
    languages: [ 'clang', 'csharp', 'java', 'javascript', 'pynthon' ],
    shell: [ 'bash', 'cmd', 'powershell' ],
    version-control-system: 'git';
  ]
```
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Anderson Ramos | Developer Profile</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0d1117;
            color: #e6edf3;
            font-family: Arial, Helvetica, sans-serif;
            padding: 40px 20px;
        }

        .container {
            max-width: 1000px;
            margin: auto;
        }

        header {
            border-bottom: 1px solid #30363d;
            padding-bottom: 25px;
            margin-bottom: 30px;
        }

        .terminal {
            color: #3fb950;
            font-family: monospace;
            margin-bottom: 15px;
        }

        h1 {
            font-size: 32px;
            margin-bottom: 10px;
        }

        h2 {
            font-size: 20px;
            margin-bottom: 20px;
        }

        h3 {
            font-size: 16px;
            margin-bottom: 15px;
            color: #58a6ff;
        }

        .subtitle {
            color: #8b949e;
            font-size: 16px;
        }

        .profile {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 35px;
        }

        .card {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 10px;
            padding: 22px;
        }

        .card-title {
            color: #8b949e;
            font-size: 13px;
            margin-bottom: 12px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .card-value {
            font-size: 22px;
            font-weight: bold;
            color: #3fb950;
        }

        .contact a {
            display: block;
            color: #58a6ff;
            text-decoration: none;
            margin-top: 12px;
            overflow-wrap: anywhere;
        }

        .contact a:hover {
            text-decoration: underline;
        }

        .technologies {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .tech-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .tech {
            background: #21262d;
            color: #c9d1d9;
            border: 1px solid #30363d;
            padding: 7px 11px;
            border-radius: 6px;
            font-size: 13px;
        }

        .tech:hover {
            border-color: #3fb950;
            color: #3fb950;
        }

        .code-block {
            background: #010409;
            border: 1px solid #30363d;
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 30px;
            overflow-x: auto;
        }

        .code-block pre {
            color: #8b949e;
            font-family: "Courier New", monospace;
            font-size: 13px;
            line-height: 1.8;
            white-space: pre-wrap;
            overflow-wrap: anywhere;
        }

        .keyword {
            color: #ff7b72;
        }

        .variable {
            color: #d2a8ff;
        }

        .string {
            color: #a5d6ff;
        }

        .comment {
            color: #8b949e;
        }

        footer {
            border-top: 1px solid #30363d;
            margin-top: 35px;
            padding-top: 20px;
            text-align: center;
            color: #8b949e;
            font-size: 13px;
        }

        footer span {
            color: #3fb950;
        }
    </style>
</head>

<body>

    <main class="container">

        <header>
            <div class="terminal">
                &gt; developer_profile.init()
            </div>

            <h1 id="authorName">Anderson Ramos</h1>

            <p class="subtitle">
                Developer Profile | Technologies & Tools
            </p>
        </header>

        <section class="profile">

            <article class="card contact">
                <div class="card-title">Contact Information</div>

                <h2>Let's connect!</h2>

                <a id="email" href="mailto:andersonramos07@live.com">
                    andersonramos07@live.com
                </a>

                <a id="linkedin"
                   href="https://www.linkedin.com/in/anderson-ramos07/"
                   target="_blank"
                   rel="noopener noreferrer">
                    LinkedIn Profile
                </a>
            </article>

            <article class="card">
                <div class="card-title">GitHub Repositories</div>

                <div class="card-value">
                    <span id="repositories">28</span>
                </div>

                <p class="subtitle" style="margin-top: 10px;">
                    Public and personal projects
                </p>
            </article>

        </section>

        <section>
            <h2>Technologies & Tools</h2>

            <div class="technologies" id="technologyContainer"></div>
        </section>

        <section style="margin-top: 35px;">
            <h2>Profile Object</h2>

            <div class="code-block">
                <pre id="profileCode"></pre>
            </div>
        </section>

        <footer>
            Built with <span>HTML</span>, <span>CSS</span> and
            <span>JavaScript</span>.
        </footer>

    </main>

    <script>
        // ----- Profile Class -----

        class Profile {
            constructor() {
                this.authorName = "Anderson Ramos";
                this.email = "andersonramos07@live.com";
                this.networking = "in/anderson-ramos07";

                this.repositories = 28;

                this.technologies = {
                    "API Tools": [
                        "Browser DevTools",
                        "Insomnia",
                        "Postman"
                    ],

                    "Container Platforms": [
                        "Docker",
                        "Kubernetes (K8s)"
                    ],

                    "Cloud": [
                        "Oracle Cloud Infrastructure (OCI)"
                    ],

                    "IDEs": [
                        "IntelliJ IDEA",
                        "VS Code",
                        "Eclipse",
                        "Android Studio"
                    ],

                    "Languages": [
                        "C",
                        "C#",
                        "Java",
                        "JavaScript",
                        "Python"
                    ],

                    "Shell": [
                        "Bash",
                        "CMD",
                        "PowerShell"
                    ],

                    "Version Control System": [
                        "Git"
                    ]
                };
            }
        }

        // ----- Instantiate Profile -----

        const in_github = new Profile();


        // ----- Render Profile Information -----

        document.getElementById("authorName").textContent =
            in_github.authorName;

        document.getElementById("email").textContent =
            in_github.email;

        document.getElementById("repositories").textContent =
            in_github.repositories;

        const linkedin = document.getElementById("linkedin");

        linkedin.href =
            "https://www.linkedin.com/" + in_github.networking;


        // ----- Render Technologies -----

        const technologyContainer =
            document.getElementById("technologyContainer");

        for (const [category, technologies]
            of Object.entries(in_github.technologies)) {

            const card = document.createElement("article");

            card.className = "card";

            const title = document.createElement("h3");

            title.textContent = category;

            const list = document.createElement("div");

            list.className = "tech-list";

            technologies.forEach(technology => {
                const item = document.createElement("span");

                item.className = "tech";
                item.textContent = technology;

                list.appendChild(item);
            });

            card.appendChild(title);
            card.appendChild(list);

            technologyContainer.appendChild(card);
        }


        // ----- Render JavaScript Representation -----

        const profileCode = document.getElementById("profileCode");

        profileCode.textContent = `class Profile {
    constructor() {
        this.authorName = "${in_github.authorName}";
        this.email = "${in_github.email}";
        this.networking = "${in_github.networking}";
        this.repositories = ${in_github.repositories};
        this.technologies = ${JSON.stringify(
            in_github.technologies,
            null,
            8
        )};
    }
}

const in_github = new Profile();`;
    </script>

</body>

</html>
