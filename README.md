# Olá, Bem vindo 👋 / Hi, welcome 👋 / Hola, bienvenido 👋 / Bonjour bienvenue 👋 / हैलो आपका स्वागत है 👋

🔍 Confira meu perfil em PDF: [Português do Brasil](202308-Curriculum-AndreAbreu.pdf), [English - USA](202308-Curriculum-AndreAbreu-EN.pdf)

## 🧑‍💻 Sobre Mim (About Me)
Eu sou André Abreu, um desenvolvedor apaixonado por tecnologia e inovação. Recentemente, tenho me aprofundado ainda mais em Go, explorando goroutines, Docker e práticas de CI/CD, sem deixar de lado minha base sólida em PHP, Python, VueJS, entre outras tecnologias.

```go
package main

import (
	"play.ground/profile"
)

func main() {
	me := profile.NewBio("Andre Abreu", "Desenvolvedor Go e Entusiasta de Tecnologia")
	stack := profile.NewStack(
		[]string{"Go (Goroutines, Docker, CI/CD)", "PHP com Laravel e Symfony", "Python / IoT", "VueJS/NodeJS/Javascript", "C++", "Ruby on Rails", "Shellscript"},
		[]string{"Postgres", "Mysql", "SQLite", "MongoDB", "DocumentDB", "Redis", "ElasticSearch", "DynamoDB", "FireBase", "FireStore"},
		[]string{"Docker", "Kubernets", "AWS", "Google Cloud Platform"},
		[]string{"Kanban", "Clean Code", "DevOps", "Linux", "Git/Bitbucket/CodeCommit", "Jira", "Confluence", "Trello", "Slack", "Telegram"},
		[]string{"LPIC 1/2/3", "CCNA/E", "CompTIA Security+", "Stonegate", "EMC+", "AWS", "Google Cloud Platform"},
		[]string{"Pai de Menina", "Marido Apaixonado", "Fotógrafo", "Aventureiro", "Marceneiro", "H.O.G."},
		[]string{"Trabalho em Equipe", "Bom Relacionamento", "Persistência", "Bom Humor"},
	)

	fmt.Println(me, stack)
}

// go.mod
module play.ground

// profile/profile.go
package profile

type Bio struct {
	Name        string
	Description string
}

type Stack struct {
	Languages    []string
	Databases    []string
	Environment  []string
	SideSkills   []string
	Certificates []string
	Hobbies      []string
	Personality  []string
}

func NewBio(name, description string) *Bio {
	return &Bio{Name: name, Description: description}
}

func NewStack(languages, databases, environment, sideSkills, certificates, hobbies, personality []string) *Stack {
	return &Stack{Languages: languages, Databases: databases, Environment: environment, SideSkills: sideSkills, Certificates: certificates, Hobbies: hobbies, Personality: personality}
}
