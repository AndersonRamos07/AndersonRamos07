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
/**
 * @file README.md
 * @description Perfil de Desenvolvedor(a)
 * @author Seu Nome <seu.email@exemplo.com>
 */

class Developer {
  constructor() {
    this.name = 'Seu Nome';
    this.role = 'Full Stack Developer';
    this.location = 'São Paulo, BR';
    this.code = ['JavaScript', 'TypeScript', 'Node.js', 'React'];
    this.status = 'Pronto para novos desafios 🚀';
  }

  sayHello() {
    return 'Olá, mundo! Obrigado por visitar meu perfil.';
  }

  getContact() {
    return {
      github: 'https://github.com',
      linkedin: 'https://linkedin.com',
      email: 'seu.email@exemplo.com'
    };
  }
}

// Executando a instância
const dev = new Developer();
console.log(dev.sayHello());
