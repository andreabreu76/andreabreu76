# Olá, Bem vindo 👋 / Hi, welcome 👋 / Hola, bienvenido 👋 / Bonjour bienvenue 👋 / हैलो आपका स्वागत है 👋

🔍 Confira meu perfil em PDF: [Português do Brasil](202308-Curriculum-AndreAbreu.pdf), [English - USA](202308-Curriculum-AndreAbreu-EN.pdf)

## 🧑‍💻 Sobre Mim (About Me)
Eu sou André Abreu, um desenvolvedor apaixonado por tecnologia e inovação. Recentemente, tenho me aprofundado ainda mais em Go, explorando goroutines, Docker e práticas de CI/CD, sem deixar de lado minha base sólida em PHP, Python, VueJS, entre outras tecnologias.

```go
package main

import (
	"fmt"
	"play.ground/profile"
)

func main() {
	me := profile.NewBio(
		"André Abreu",
		"Desenvolvedor Go, DevOps, e Entusiasta de Tecnologia e Inovação",
	)

	stack := profile.NewStack(
		[]string{"Go (Goroutines, Fiber, Docker, CI/CD)", "PHP (Laravel, Symfony)", "Python (Django, IoT)", "VueJS/NodeJS/JavaScript", "C++", "Ruby on Rails", "Shellscript"},
		[]string{"Postgres", "MySQL", "SQLite", "MongoDB", "DocumentDB", "Redis", "ElasticSearch", "DynamoDB", "Firebase", "Firestore"},
		[]string{"Docker", "Kubernetes", "AWS (Terraform, ECS, S3, Lambda)", "Google Cloud Platform", "GitHub Actions", "GitLab CI/CD"},
		[]string{"Kanban", "Scrum", "Clean Code", "DevOps", "Linux (LPIC 1/2/3)", "Git/Bitbucket/CodeCommit", "Jira", "Confluence", "Trello", "Slack", "Telegram"},
		[]string{"LPIC 1/2/3", "CCNA/E", "CompTIA Security+", "Stonegate", "EMC+", "AWS Certified", "Google Cloud Certified"},
		[]string{"Pai de Menina", "Marido Apaixonado", "Motociclista (H.O.G.)", "Fotógrafo", "Aventureiro", "Marceneiro"},
		[]string{"Trabalho em Equipe", "Empatia", "Resiliência", "Persistência", "Bom Humor", "Comunicação Eficiente"},
	)

	fmt.Println(me)
	fmt.Println(stack)
}
```

go.mod
```go
module play.ground
```

profile/profile.go
```go
package profile

import "fmt"

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
	return &Stack{
		Languages:    languages,
		Databases:    databases,
		Environment:  environment,
		SideSkills:   sideSkills,
		Certificates: certificates,
		Hobbies:      hobbies,
		Personality:  personality,
	}
}

func (b *Bio) String() string {
	return fmt.Sprintf("👤 Nome: %s\n💼 Descrição: %s\n", b.Name, b.Description)
}

func (s *Stack) String() string {
	return fmt.Sprintf(`
📚 Linguagens: %v
🗄️ Bancos de Dados: %v
⚙️ Ambientes/Infraestrutura: %v
🎯 Habilidades Adicionais: %v
📜 Certificações: %v
🎨 Hobbies: %v
🌟 Personalidade: %v
`, s.Languages, s.Databases, s.Environment, s.SideSkills, s.Certificates, s.Hobbies, s.Personality)
}
```
