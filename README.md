# 0x0B. Implement a design with bootstrap

In this project, you will implement 3 web pages with Bootstrap. You will use all HTML/CSS/Accessibility/Responsive design/Bootstrap knowledges that you learned previously.

You won’t have a lot of instruction, you are free to implement it the way that you want - the objective is simple: Have fully functional web pages that look the same as the designer file.

Here the final result:

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/3c71cc99d2fc1c12a3d3.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=111ceca128329ee5530970e8d6558f60fdd8f384cfa30b149dc168ed1c634c38)

This webpage has been designed by Nicolas Philippot, UI/UX designer. You can find final screens  [here](https://intranet-projects-files.s3.amazonaws.com/holbertonschool-webstack/623/Archive.zip "here")

### Requirements

-   You have to use Bootstrap
-   Your  `styles.css`  must be as small as you can -  **you must use as much as you can Bootstrap classes**

### Imports

For this project, you will need: fonts from Google, JQuery, Bootstrap CSS/JS

```html
<link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Coiny&display=swap" rel="stylesheet">

<script src="https://code.jquery.com/jquery-3.4.1.min.js" integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo=" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>

<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">

```

## Tasks

### 0. Read and be familiar with Figma


Create an account in  [Figma](https://intranet.hbtn.io/rltoken/0OS4ME4Kjnw0I82IVkkoSw "Figma")  and open these files:

-   [Homepage](https://intranet.hbtn.io/rltoken/RLej4Ua6W3EmDh7UCwGTzQ "Homepage")  -  [fig file](https://intranet.hbtn.io/rltoken/1ZTxYF-usvxpIjj44YYcyw "fig file")
-   [Pricing](https://intranet.hbtn.io/rltoken/xQCL77_ePGWntUAe4T7ebQ "Pricing")  -  [fig file](https://intranet.hbtn.io/rltoken/AdJ6ZyZrG90gRNAI5bt_lA "fig file")
-   [Courses](https://intranet.hbtn.io/rltoken/__3w9ryapSUAwMaAYYS6ZA "Courses")  -  [fig file](https://intranet.hbtn.io/rltoken/1JL-gCkfJ5Hqb0Sf2lmymw "fig file")

And “Duplicate to your Drafts” to have access to all design details.

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/559ad8d43fb61e310e2b.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=71395186206bca311505ced4c51aa4dbe8b24051b13844cae3f87dca1332aaac)

Important notes with Figma:

-   if your computer doesn’t have missing fonts, you can find them here:  [source-sans-pro](https://intranet.hbtn.io/rltoken/4uQkoVbAjr7lRVqSVCWBcw "source-sans-pro")  and  [Spin-Cycle-OT](https://intranet.hbtn.io/rltoken/5HnXzrMbtVKLCScrdy4CIg "Spin-Cycle-OT")
-   some values are in float - feel free to round them
-   “Be pixel perfect” - yes! but mainly make sure colors, size and position are correct.  #C271FF  is not  purple.

For this task, please write an amazing  `README.md`

**Interactions note:**

-   Web pages must switch to the tablet version when the screen width is 768px
-   Web pages must switch to the mobile version when the screen width is 576px
-   button hover/active:  `opacity: 0.9`

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `README.md`


### 1. Header first



Let’s start by the Homepage:  **create the header/hero piece**

Here an archive of all assets needed (for the entire project):

-   [images_images.zip](https://holbertonintranet.s3.amazonaws.com/uploads/misc/2020/3/e62e701b6ce0374555e9.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=345600&X-Amz-SignedHeaders=host&X-Amz-Signature=ac8f881bd83fac6f422230586b180aa2cf488681aed26317d1e610cb6f3070b6 "images_images.zip")
-   [holberton_school-icon.zip](https://holbertonintranet.s3.amazonaws.com/uploads/misc/2020/3/7159d988278de54d859d.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=345600&X-Amz-SignedHeaders=host&X-Amz-Signature=b502770bf639d768b70d10cb9fde3db7119629257896560b0820d99330aa1b11 "holberton_school-icon.zip")

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/4/13572c3773e26651761e8b4a74b3383300ed9563.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d2696a19326e81974b866955c3ace845c28f67b0df273327d8200e50e4bfec12)

**Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/8854d68a957ef7dc2315.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=365a93a80e59df4f74f114f079b4f0165e48a12580a37df10deeb2d94373bce8)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `0-homepage.html, styles.css`


### 2. Carousel of quotes



**Create the section “Carousel of quotes”**

By using a Carousel component of Bootstrap, create this Carousel of quotes.

You can have for the moment one quote or twice the same for testing (like example below)

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/8455560f9ac188658195.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2b853b3cbd9f6b3d881e59b1afdfbcab1d9606fb95844148a2ca90d8d7090be9)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `1-homepage.html, styles.css`


### 3. Popular videos



**Create the section “Most popular tutorials”**

By using a Carousel component of Bootstrap, create this Carousel of video cards.

**Reminder:**

-   Desktop: 4 cards
-   Tablet: 2 cards
-   Mobile: 1 card

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/4b610dc2d2cc17ceb2f7.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b00c98287019ffd4d017991e1877402f7128b134bcd2c174192e7374ad40b345)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `2-homepage.html, styles.css`


### 4. Row of smiles



**Create the section “Free membership”**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/970efd54768b693bbfac.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=a400e0e615e37e1d3b57ac4aec6407ec08e7f304cf163dbd9ee2424e475f60ef)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `3-homepage.html, styles.css`


### 5. Latest videos



**Create the section “Latest videos”**

Copy the block “Most popular tutorials” to “Latest videos”

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `4-homepage.html, styles.css`


### 6. ... and the footer!


**Create the footer**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/739d7cc60098e7ff8f25.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8e0aaaeb95c47db7585a7b734392abe4200a0a0e0b1b00d01c41f04ea5674fb7)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `homepage.html, styles.css`


### 7. Pricing - header



Now, let’s do the pricing page:  **create the header/hero piece**

The mobile version must be the same as the Homepage - it’s time to reuse code!

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/ccd30a4d80a990b96740.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004002Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=465fd4d3b806b54190d6358c9a7d59eb3628f71858938aaa3167c63c1185b8d4)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `0-pricing.html, styles.css`


### 8. Prices grid



**Create the prices grid**

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/0ac3872946a0014e4f99.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=11b125db248d1c144ca1a24394629268ab611b33c140b93543d14a8ff2f66ca0)

**Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/edea8172b9cc0a867237.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=824fe4e7a89404cf05f2758d2ef2d44051674be1ae60ebf6d8cee3eb2700569a)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `1-pricing.html, styles.css`


### 9. Quotes section



Same as the Homepage,  **create the Carousel of quotes**

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `2-pricing.html, styles.css`


### 10. FAQ



**Create the FAQ grid**

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/db8f90e37593a29c1ab6.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ac3294727e4881275f0d5af906bf51b23d29197a0ba4a06b076cd6857afb1035)

**Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/eaeb117d40690a451c7b.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7c2e4913834bf4d2a0d4a20c74028ffddf67746872fb1696559d51f639677d45)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `3-pricing.html, styles.css`


### 11. Close the page with a footer



Same as Homepage,  **create the footer**

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `pricing.html, styles.css`


### 12. Courses - header



Now, let’s do the courses page:  **create the header/hero piece**

The mobile version must be the same as the Homepage - it’s time to reuse code!

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/a5ba265af5dd643ad942.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=cfed937049fa6d318ba979461e4756c4f1594bb2a52b8498755efdf4ebebfc84)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `0-courses.html, styles.css`


### 13. Search filters

**Create the search filters section**

Dropdown is a nice way to create filters.

For the selected/placeholder value of both dropdown, no need to have dynamic value - static content is totally ok.

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/98c0564e59ec5620990e.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e2952ed8da901738168a84c1f7953bf22e379bd6f8a7a56350077ec892310550)

**Tablet/Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/3627550eccca7958d390.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d3c39d2223ffa5394388e06680f9afdc05b082478fa69d05910abba73fba874b)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `1-courses.html, styles.css`


### 14. List of result



**Create the result section of courses**

You can reuse the same cell for testing. Don’t forget to test with odd and even number of cells.

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/76b2074f3f6bbd25cdb9.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220510%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220510T004003Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ef02b83a62c498d1898f072fde7142ef676be21b725ec5de0e55eeea976daa77)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `2-courses.html, styles.css`


### 15. Close the page with a footer



Same as Homepage and Pricing page,  **create the footer**

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `courses.html, styles.css`




Copyright © 2022 Holberton Inc, All rights reserved.