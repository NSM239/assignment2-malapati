# MALAPATI NAVYA SRI
i have done my bachelors in electronics and communication engineering at chalapathi institute of technology.

![Aboutme](/WhatsApp%20Image%202023-02-01%20at%2019.14.58.jpeg)

---
# Trip
I am exploring country to have a good experience with lot of people.

|  **Country**  |  **Reason to visit**  |  **Number of days** |
|---------------|-----------------------|---------------------|
|  USA          |  To visit places      |  5                  |
|  UK           |  To see parks         |  4                  |
|  Itali        |  To Visit relatives   |  15                 |
|  Japan        |  To visit friends     |  10                 |

# photy Quotes

>It's not true that I had nothing on.I had the radio on. -_Marilyn Monroe_
>
>When life gives you lemons,squirt someone in the eye.-_Cathy Guiswite_

---

# code Fencing

> How to do Placing Items on a Circle?

[link](https://stackoverflow.com/questions/66930181/how-to-place-icons-at-the-edge-of-circle)

Sass
```
@mixin on-circle($item-count, $circle-size, $item-size) {
  position: relative;
  width:  $circle-size;
  height: $circle-size;
  padding: 0;
  border-radius: 50%; 
  list-style: none;       
  
  > * {
    display: block;
    position: absolute;
    top:  50%; 
    left: 50%;
    width:  $item-size;
    height: $item-size;
    margin: -($item-size / 2);
  
    $angle: (360 / $item-count);
    $rot: 0;

    @for $i from 1 through $item-count {
      &:nth-of-type(#{$i}) {
        transform: 
          rotate($rot * 1deg) 
          translate($circle-size / 2) 
          rotate($rot * -1deg);
      }

      $rot: $rot + $angle;
    }
  }
}

```
[link](https://css-tricks.com/snippets/sass/placing-items-circle/)