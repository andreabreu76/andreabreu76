Olá, bem vindo... 

```go
package main

import (
	"play.ground/profile"
)

func main() {
	me := profile.NewBio("Andre Abreu")
	stack := profile.NewStack(
		[]string{"PHP / Laravel", "Go", "Python / IoT", "Javascript", "C"},
		[]string{"Postgres", "Mysql", "SQLite", "MongoDB"},
		[]string{"Docker", "Kubernets", "AWS", "Azure"},
		[]string{"Vue.js"},
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
	languages []string
	databases []string
	misc      []string
	ongoing   []string
}
func NewBio(name string) *Bio {
	return &Bio{name}
}
func NewStack(languages, databases, misc, ongoing []string) *Stack {
	return &Stack{languages, databases, misc, ongoing}
}
```
