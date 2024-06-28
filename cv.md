# Zilola Nazarova
<img src="profile-photo.jpg" width="150">

## Contacts
E-mail: ziloladev@gmail.com  
Telegram: [@ZilolaDev](https://t.me/ZilolaDev)  
LinkedIn: [in/zilola-nazarova](https://www.linkedin.com/in/zilola-nazarova/)  
GitHub: [Zilola-Nazarova](https://github.com/Zilola-Nazarova)  
Discord: [nazarovazi](https://discordapp.com/users/1132805236575187075), rs-school: `Zilola (@Zilola-Nazarova)`

## About Me
Full-stack web developer blending a background in architecture with a passion for UX/UI design, bringing a unique perspective to software development. Skilled in Ruby on Rails, React, and JavaScript, with proven ability in pair programming and thriving in remote environments. Demonstrates strong mathematical and artistic aptitude, excelling in problem-solving and creative solutions. A fast learner and effective multitasker, eager to leverage comprehensive skills in technology to contribute to innovative projects.

## Skills
**Front-End:** JavaScript (ES5/ES6), React, Redux, jQuery, HTML5, CSS3, Bootstrap 5  
**Back-End:** Ruby, Rails, PostgreSQL, Node.js, MongoDB, Express  
**Tools & Methods:** Git, GitHub, Netlify, Mobile/Responsive Development, Jest, RSpec, TDD, Chrome Dev Tools  
**Professional:** Remote Pair-Programming, Teamwork  
**Graphical:** Adobe Photoshop, Adobe Illustrator, CorelDraw, Figma  

## Code Sample
**Simple Quicksort:** A `partition` method splits an array into smaller and greater elements (with respect to the first element aka `pivot`). Each time I call `partition`, I am sorting two parts of the array with respect to each other. I repeatedly use `partition` on sub-arrays (left and right) to sort an entire array. When `partition` is called on two elements, that sub-array is fully sorted. The first element in any sub-array is used as a pivot. It appears in the middle when combining the two lists together (`resemble` method).
<details>
<summary>SHOW CODE</summary>

```ruby
def simple_quicksort(array)
  partition(array)
end

def partition(array)
  pivot = array[0]
  before, after = [], []
  (1..array.length - 1).each do |i|
    if array[i] <= pivot
      before.push(array[i])
    elsif array[i] > pivot
      after.push(array[i])
    end
  end
  before = partition(before) if before.length > 1
  after = partition(after) if after.length > 1
  resemble(before, pivot, after, array)
end

def resemble(before, pivot, after, array)
  index = 0
  array, index = join_part(before, index, array)
  array[index] = pivot
  index += 1
  array, index = join_part(after, index, array)
  array
end

def join_part(part, index, array)
  until part.empty?
    array[index] = part[0]
    index += 1
    part.shift
  end
  [array, index]
end
```
</details>

## Experience
**ITRANSITION**  
_Intern JavaScript Developer, Remote_  
_April 2024 – June 2024_
- Developed a full-stack MERN project integrated with 2 services (Jira, Odoo). [Live Demo](https://itransition-courseproject-frontend.onrender.com/) \| [GitHub](https://github.com/Zilola-Nazarova/itransition-courseproject) \| [Certificate](https://drive.google.com/file/d/1r8X-kzND5sdMxpGS1UiWIZJebz-6UX25/view?usp=sharing)

**HIGHLIGHTED PERSONAL PROJECTS**  
_Full Stack Web Developer_  
_May 2023 – March 2024_
- _SmartPocket_ — keep track of your expenses — create, update, delete transactions and group them into categories. Built with: Ruby on Rails. [Live Demo](https://smart-pocket-app.onrender.com/) \| [GitHub](https://github.com/Zilola-Nazarova/budget-app)
- _Mountains Forecast_ — see current weather conditions and hourly forecasts for peaks; add new locations. Built with: React, Redux and Ruby on Rails. [Live Demo](https://mountains-forecast.onrender.com/) \| [GitHub](https://github.com/Zilola-Nazarova/mountains-forecast)
- _Bookstore_ — create your list of favorite books by adding and removing books. The list is saved in local storage. Built with: React, Redux. [Live Demo](https://bookstore-4xzu.onrender.com/) \| [GitHub](https://github.com/Zilola-Nazarova/bookstore)

**TOSHUYJOYLITI**  
_Tashkent, Uzbekistan_  
_Architect, Aseismic Construction Department_  
_Apr 2019 – May 2023_
- Rendered models of innovative constructions which were presented at the UzBuild 2020 exhibition.
- Performed calculations and documentation of innovative constructions that were patented internationally (IAP
20180364).
- Earned a promotion over 1 year for updating 8 building codes (approved by the Ministry of Construction).

## Education
**MICROVERSE**  
_Full Stack Web Development Program, Full-Time, Remote_  
_May 2023 – Dec 2023_
- Spent 1300+ hours mastering algorithms, data structures, and full-stack development while simultaneously developing projects with Ruby, Rails, JavaScript, React, and Redux.
- Developed skills in remote pair programming using GitHub, industry-standard git-flow, and daily standups to communicate and collaborate with international remote developers.

**TASHKENT UNIVERSITY OF ARCHITECTURE AND CIVIL ENGINEERING**  
_Tashkent, Uzbekistan_  
_Bachelors, Architecture (GPA 3.55)_  
_Sep 2013 – Feb 2018_
- Was chosen as 1 of 5 students for the 1st international exchange program of the university and studied 1 semester at the Hanbat National University (South Korea).
- Participated in governmental competitions on descriptive geometry (2016 - 4th place) and architectural design (2016 - 2nd place, 2017 - 2nd place), was granted a 2nd-grade diploma in 'Architecture Universities Best Diploma Projects in 2017-2018' by the Union of Architects of Uzbekistan.

## English
CERTIFICATES
- IELTS Academic - 7.0 (2013)
- TOEFL iBT - 107 (2015)

PRACTICE
- 6-month exchange program study in South Korea (2015)
- a month exchange program study in France (March 2016)
- 8-months remote learning at Microverse BootCamp (2023)

OTHER
- EPAM Campus English test - B2
