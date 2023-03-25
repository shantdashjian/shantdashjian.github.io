---
title: "Spring Slice Tests, Mocking, and Gradle" # Title of the blog post.
date: 2023-03-25T07:34:19-07:00 # Date of post creation.
featured: true # Sets if post is a featured post, making appear on the home page side bar.
codeMaxLines: 10 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: false # Override global value for showing of line numbers within code block.
figurePositionShow: true # Override global value for showing the figure label.
tags:
  - spring
  - mockito
  - mocking
  - gradle
  - slice tests
# comment: false # Disable comment if false.
---
## Spring
I continue studying for the Spring certification. Yesterday, I reviewed:
1. Adding a GET endpoint and testing it with `TestRestTemplate`
2. Separating concerns using `Spring Data` and the Repository pattern
3. Using `Optional`

## Slice Tests
Spring Boot provides a way for [test slicing](https://spring.io/blog/2016/08/30/custom-test-slice-with-spring-boot-1-4). Yesterday, I practiced using `@WebMvcTest` and 
`MockMvc` to 
slice the 
testing to include only the web layer. For that, mocking with `Mockito` comes in handy with functions like `when`, 
`thenReturn`, and `verify`.

## Gradle
You can tell Gradle to only run certain tests. Like this:
`./gradlew test --tests example.cashcard.CashCardControllerTest`
