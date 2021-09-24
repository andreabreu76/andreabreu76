Olá, Bem vindo 👋 / Hi, wellcome 👋 / Hola, bienvenido 👋 / Bonjour bienvenue 👋 / हैलो आपका स्वागत है 👋 

```go
package main

import (
	"play.ground/profile"
)

func main() {
	me := profile.NewBio("Andre Abreu")
	stack := profile.NewStack(
		[]string{"PHP / Laravel", "Go", "Python / IoT", "VueJS/NodeJS/Javascript", "C", "Shellscript"},
		[]string{"Postgres", "Mysql", "SQLite", "MongoDB"},
		[]string{"Docker", "Kubernets", "AWS", "Azure"},
		[]string{"Kambam","Cleancode","DevOPS", "Linux", "Git/Bitbucket/CodeCommit"},
		[]string{"LPIC 1/2/3","CCNA/E", "Compitia Secure+", "Stonegate", "EMC+", "AWS"}
		[]string{"Girl father","Husband in love","Photographer","Outlander/Camper","Woodworker"}
		[]string{"Colaborative team work","Good relationship","Peart", "Good tempered"}
	)
	_ = me
	_ = stack
}

-- go.mod --
module play.ground

-- profile/profile.go --
package profile

type Bio struct {
	Name string
}
type Stack struct {
	languages    []string
	databases    []string
	ambient      []string
	sideSkills   []string
	certificates []string
	hobbys	     []string
	personality  []string		
}
func NewBio(name string) *Bio {
	return &Bio{name}
}
func NewStack(languages, databases, misc, ongoing []string) *Stack {
	return &Stack{languages, databases, ambient, sideSkills, certificates, hobbys, personality}
}
```
My Stats

**My GitHub Stats**
 <div>
  <a href="https://github.com/andreabreu76">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=andreabreu76&show_icons=true&theme=nord&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=andreabreu76&layout=compact&langs_count=7&theme=nord"/>
  </a>
</div>
<br>
