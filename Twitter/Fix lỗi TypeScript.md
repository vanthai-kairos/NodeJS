# Cách fix lỗi  ** TypeScript**

Lỗi TypeScript thường liên quan đến kiểu dữ liệu không đúng 
```typescript
interface User{
    name:string
    age:number
}

const render=(user:User)=>{
    console.log(user)
}

const user={name:'Van Thai'}
render(user)
```
Có thể bypass bằng `as any` như sau 

```typescript
interface User{
    name:string
    age:number
}

const render=(user:User)=>{
    console.log(user)
}

const user={name:'Van Thai'}
render(user as any)

```