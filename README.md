# notification-component

> Simple Vue.js notification component using [bulma](https://bulma.io/documentation/) CSS framework.
>

## Example
```
<app-notification
    notification-type="is-danger"
    v-if="showNotification"
    @close-notification="showNotification=$event">

    Primar lorem ipsum dolor sit

 </app-notification>
```
>Only need to be set `notification-type` from one of classes from bulma CSS framework.
```
 is-primary
 is-link
 is-info
 is-success
 is-warning
 is-danger
```
>`notification-type` can be bind:
 ```
 <app-notification
     :notification-type="'is-danger'"
     v-if="showNotification"
     @close-notification="showNotification=$event">

     Primar lorem ipsum dolor sit

  </app-notification>
 ```

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```
