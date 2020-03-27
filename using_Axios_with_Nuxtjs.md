[Nuxt Axios](https://axios.nuxtjs.org/)

Setting the header -
`this.$axios.setHeader('Authorization', 'Bearer ' + mytoken)`

Make a HTTP GET call -
`this.$axios.get('http://localhost/api')`

Getting the result -
`.then(response => {
     this.datalist = response.data
  })`

Error handing - 
`.catch(error => {
          this.loading = false
          console.log(error)
        })`
        
### Sample code

```
const mytoken = "BJYVJHvjvUJVJG..."
this.$axios.setHeader('Authorization', 'Bearer ' + mytoken)
this.$axios.get('http://localhost/api')
  .then(response => {
     consol.log(response.data)
   })
   .catch(error => {
     console.log(error)
   })
```
