### Hi I'm Adriel š

```tsx
import React from 'react'
import ReactDOM from 'react-dom/client'

interface MyProps {
    name:string,
    languages:string[],
    hobbies:string[],

}


const AdrielDev = (props:MyProps) => {
  return (
    <>
    <h1>{props.name}Dev</h1>
    <p>I am currently familiar with the following languages or frameworks</p>
    <ul>
    {
      props.languages.map(lenguage=> <li>{lenguage}</li>)
    }
    </ul>

    <article>
      <p>I also like</p>
      {
        props.hobbies.map(hobbie=> <p>{hobbie}</p>)
      }
    </article>
    </>
  )
}

const languages:string[] = ['Javascript','Typescript','React','Java','node','nestJS']

const hobbies:string[] = ['climb','coffe','program']


ReactDOM.createRoot(document.getElementById('root')!).render(
  <React.StrictMode>
    <AdrielDev name='Adriel' languages={languages} hobbies={hobbies}/>
  </React.StrictMode>
)



```

<!--
**adriel87/adriel87** is a āØ _special_ āØ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- š­ Iām currently working on ...
- š± Iām currently learning ...
- šÆ Iām looking to collaborate on ...
- š¤ Iām looking for help with ...
- š¬ Ask me about ...
- š« How to reach me: ...
- š Pronouns: ...
- ā” Fun fact: ...
-->
