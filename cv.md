# Alexey Vasileuski

---

## Contacts
**Phone** [+375 (29) 9 050 737](tel:+375299050737)

**Email** [alex.vasilevski007@gmail.com](mailto:alex.vasilevski007@gmail.com)

**Discord** [vasilevsky_a#5738](https://discordapp.com/users/332215070253645834/)

**Telegram** [@vasilevsky_a](https://t.me/vasilevsky_a)

---

## About myself
In 2020 I've enrolled in Belarusian State University of Informatics and Radio-electronics to the faculty of Computer Systems and  Networks.
Since now I'm a third-year student, I've learned a lot in computer science, like arithmetic and logic fundament of computer technology, architecture of personal computers, low-level programming on assembler, system software of computing machines, software testing and development, cross-platform programming, theory of computer networks, interfaces and peripheral devices.
As I am currently interested in developing end-user applications, I am studying now Swift and JavaScript languages to develop native iOS (SwiftUI) and web applications respectively.
### Skills and Proficiency:
* C / C++
  + Linux system programming
  + Windows devices and interfaces programming
  + Windows networking programming
  + Visual Studio, Clion
* Java
  + Cross-platform app development for JVM
  + Back-end Spring development
  + Intellij Idea
* iOS/iPadOS/MacOS development (currently learning)
  + Swift programming language
  + SwiftUI framework
  + Xcode
* Front-end Web development (currently learning)
  + HTML5, CSS3
  + JavaScript
  + WebStorm
* Git, GitHub
* Trello, PlanningPoker
* Figma
### Code example
*Extension to **View** that turns it into a card:*

```Swift
import SwiftUI

struct Cardify: ViewModifier {
    var isFaceUp: Bool
    var isMatched: Bool

    func body(content: Content) -> some View {
        ZStack {
            let shape = RoundedRectangle(cornerRadius: DrawingConstants.cardCornerRadius)
            if isFaceUp{
                shape.fill().foregroundColor(.white)
                shape.strokeBorder(lineWidth: DrawingConstants.borderWidth)
            } else {
                shape.fill()
            }
            content
                .opacity(isFaceUp ? 1 : 0)
            if isMatched {
                shape.opacity(DrawingConstants.matchedOpacity)
            }
        }
    }
    
    private struct DrawingConstants {
        static let borderWidth: CGFloat = 3
        static let cardCornerRadius: CGFloat = 12
        static let matchedOpacity: CGFloat = 0.5
    }
}

extension View {
    func cardify(isFaceUp: Bool, isMatched: Bool) -> some View {
        self.modifier(Cardify(isFaceUp: isFaceUp, isMatched: isMatched))
    }
}
```
### Education
* Belarusian State University of Informatics and Radio-electronics, Faculty of Computer Systems and Networks, speciality Computing machines, systems and networks: System Engineer (now on the 6th semester)
* Courses:
  + Stanford University's course [CS193p](https://cs193p.sites.stanford.edu): Developing Applications for iOS using SwiftUI (in progress)
  + [R S School JS / Front-end](https://rs.school/js/): Stage 1 (in progress)

### Languages
* English: Intermediate/Upper-intermediate
* Russian: Native
* Belarusian: Intermediate