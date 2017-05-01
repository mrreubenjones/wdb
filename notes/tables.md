# Tables

Colt Steele mentions the `<thead>` and `<tbody>` tags in the [HTML section of his Web Developer Bootcamp.](https://www.udemy.com/the-web-developer-bootcamp/learn/v4/t/lecture/3861218)

While I've seen these elements before (most notably in [Bootstrap implementations](https://v4-alpha.getbootstrap.com/content/tables/)) I've never really paid much attention to them. But this time I took notice, and after some digging, Today I Learned that while `<thead>` and `<tbody>` (and `<tfoot>`) don't actually provide accessibility functionality, it doesn't hurt to use them for styling purposes, and they do of course provide semantic scent.

[Web Aim](http://webaim.org/) (webaim.org) provide some great table accessibility information, and now I also know about table captions and scope. In brief, captions exist to provide a brief content summary of the table, while scope indicates the type of `<th>` header being used—row or column. Note that `<th>` can be used as the first column in a row, something I've never noticed before. Boom, as they say.

For more depth see: [webaim.org/techniques/tables/data](http://webaim.org/techniques/tables/data)

### Example from Web Aim: Shelly's Daughters.

<table>
    <caption>Shelly's daughters by birth and marriage.</caption>
    <tbody><tr>
      <td></td>
      <th scope="col">Name</th>
      <th scope="col">Age</th>
      <th scope="col">Birthday</th>
    </tr>
    <tr>
      <th rowspan="2" scope="row">by birth</th>
      <th scope="row">Jackie</th>
      <td>5</td>
      <td>April 5</td>
    </tr>
    <tr>
      <th scope="row">Beth</th>
      <td>8</td>
      <td>January 14</td>
    </tr>
    <tr>
      <th scope="row">by marriage</th>
      <th scope="row">Beth</th>
      <td>8</td>
      <td>January 14</td>
    </tr>
  </tbody>
</table>

```html
<table>
    <caption>Shelly's daughters by birth and marriage.</caption>
    <tbody><tr>
      <td></td>
      <th scope="col">Name</th>
      <th scope="col">Age</th>
      <th scope="col">Birthday</th>
    </tr>
    <tr>
      <th rowspan="2" scope="row">by birth</th>
      <th scope="row">Jackie</th>
      <td>5</td>
      <td>April 5</td>
    </tr>
    <tr>
      <th scope="row">Beth</th>
      <td>8</td>
      <td>January 14</td>
    </tr>
    <tr>
      <th scope="row">by marriage</th>
      <th scope="row">Beth</th>
      <td>8</td>
      <td>January 14</td>
    </tr>
  </tbody>
</table>
```

