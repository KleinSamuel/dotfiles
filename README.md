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

<!--
```rust
fn main() {
    let me = SoftwareEngineer {
        name: "Andreas Ellwanger",
        role: "Software Engineer",
        company: "Celonis",
        languages: Vec::from(["de_DE", "en_US"])
    };
    me.say_hi();
}

#[allow(dead_code)]
struct SoftwareEngineer<'a> {
    name: &'a str,
    role: &'a str,
    company: &'a str,
    languages: Vec<&'a str>
}

impl SoftwareEngineer<'_> {
    fn say_hi(&self) {
        println!("Thanks for dropping by, hope you find some of my work interesting. ~{}", self.name);
    }
}
```
-->
