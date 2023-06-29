# Hi 👋

```go
package githubrepo

import "fmt"

func main() {
	var me = Bioinformatician{
		name:                 "Samuel Klein",
		role:                 "PhD student",
		institution:          "LMU Munich",
		humanLanguages:       []string{"german", "english"},
		programmingLanguages: []string{"java", "python", "javascript", "go", "bash"},
	}
	me.sayHi()
}

type Bioinformatician struct {
	name                 string
	role                 string
	institution          string
	humanLanguages       []string
	programmingLanguages []string
}

func (b Bioinformatician) sayHi() string {
	return fmt.Sprintf("Thanks for dropping by, hope you find some of my work interesting!\n\ngreetings\n%s", b.name)
}
```
