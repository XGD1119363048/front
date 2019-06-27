# visual-analysis-platform-frontend

> A Vue.js project for the visual analysis platform 
> whose details and code are as follow: 
> https://github.com/cutrain/visual-analysis-platform.

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

```

## Structure

![structure](https://github.com/yjwang12/front/blob/master/src/assets/readme-structure.png)

### components 
> vue components, location: /src/components/xxx.vue 
- draggable components

> including CircleDraggable.vue, ComponentDraggable.vue, Node.vue 
> which is used in ProjectDetail.vue. 

- parameter list

> only one, paramBorder.vue used in ProjectDetail.vue

- tree table

### views 
> /src/views/xxx.vue
- index
> the parent of ProjectDetail and ProjectView
- ProjectView
> to manage the subjects created by users, using basic options. 
> A user can rename, delete and enter the project chose from the project list.
- ProjectDetail
> core 
- Database
> to manage the data uploaded

