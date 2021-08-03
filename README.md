# gatsby-remark-quizdown
Create interactive quizzes in your markdown `.mdx` files

## Installation

`npm install --save gatsby-remark-quizdown quizdown`

Then add the plugin to your `gatsby-config.js`.

```js
plugins: [
  {
    resolve: `gatsby-plugin-mdx`,
    options: {
      gatsbyRemarkPlugins: [
        {
          resolve: "gatsby-remark-quizdown",
          options: {
            
          },
        },
      ],
    },
  },
],
```

## Usage

```mdx

# Markdown processed by gatsby-plugin-mdx

<Quizdown>

# Question 1

What is the capital of Italy?

> This will be processed by the quizdown plugin!

- [ ] Rome
- [x] Berlin
- [ ] Paris
- [ ] London


</Quizdown>

```

### Credits

Inspired by `gatsby-remark-mermaid` (https://github.com/remcohaszing/gatsby-remark-mermaid) and `gatsby-mdx-tts` (https://github.com/flogy/gatsby-mdx-tts)
