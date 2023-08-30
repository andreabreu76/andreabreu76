Olá, Bem vindo 👋 / Hi, wellcome 👋 / Hola, bienvenido 👋 / Bonjour bienvenue 👋 / हैलो आपका स्वागत है 👋

My profile in pdf, [Portuguese](202308-Curriculum-AndreAbreu.pdf) [English] (202308-Curriculum-AndreAbreu-EN.pdf)

```go
package main

import (
	"play.ground/profile"
)

func main() {
	me := profile.NewBio("Andre Abreu")
	stack := profile.NewStack(
		[]string{"PHP with Laravel and Symfony", "Go with Gin and Fiber", "Python / IoT", "VueJS/NodeJS/Javascript", "C++", "Ruby on Rails", "Shellscript"},
		[]string{"Postgres", "Mysql", "SQLite", "MongoDB", "DocumentDB", "Redis", "ElasticSearch", "DynamoDB", "FireBase", "FireStore"},
		[]string{"Docker", "Kubernets", "AWS", "Google Cloud Platform"},
		[]string{"Kambam", "Cleancode", "DevOPS", "Linux", "Git/Bitbucket/CodeCommit", "Jira", "Confluence", "Trello", "Slack", "Telegram"},
		[]string{"LPIC 1/2/3", "CCNA/E", "Compitia Secure+", "Stonegate", "EMC+", "AWS", "Google Cloud Platform"},
		[]string{"Girl father", "Husband in love", "Photographer", "Outlander/Camper", "Woodworker", "H.O.G."},
		[]string{"Collaborative team work", "Good relationship", "Peart", "Good tempered"},
	)

	fmt.Println(me, stack)
}

-- go.mod --
module play.ground

-- profile/profile.go --
package profile

type Bio struct {
	Name string
}

type Stack struct {
	Languages    []string
	Databases    []string
	Ambient      []string
	SideSkills   []string
	Certificates []string
	Hobbys       []string
	Personality  []string
}

func NewBio(name string) *Bio {
	return &Bio{Name: name}
}

func NewStack(languages, databases, ambient, sideSkills, certificates, hobbys, personality []string) *Stack {
	return &Stack{Languages: languages, Databases: databases, Ambient: ambient, SideSkills: sideSkills, Certificates: certificates, Hobbys: hobbys, Personality: personality}
}
```

**My GitHub Stats**

 <div>
  <a href="https://github.com/andreabreu76">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=andreabreu76&show_icons=true&theme=nord&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=andreabreu76&layout=compact&langs_count=7&theme=nord"/>
  </a>
</div>
<br>
