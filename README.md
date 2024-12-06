- Server side actions are mainly, for now, used to perform mutations from client side as they make a POST Request

-If you want to call server Action from the client side, you'll have to create a separate file with "use server" written at the start of the file.

// lib/action.ts
"use server"

export async function mutate(){}

- To call Server action from the server side you can just write "use server" at the top of the function body.

async function handleSubmit() {
    "use server"

    ....
}

or a deeper dive into Server Actions in Next.js, check out this: https://www.youtube.com/watch?v=FKZAXFjxlJI

Server Actions Memo Project

This project demonstrates the use of Server Side Actions in Next.js 15 for handling server-side operations efficiently.

Key Features
Server Side Actions: Used primarily for performing mutations via POST requests.
Client-Server Integration: Examples of calling Server Actions from both client and server contexts.
Secure and Performant: Implements best practices for security and efficient data handling.