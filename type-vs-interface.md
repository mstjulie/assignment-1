# Type vs Interface in TypeScript

## ১. ভূমিকা (Introduction) 
TypeScript-এ type এবং interface হলো দুটি গুরুত্বপূর্ণ বিষয়। এগুলো ব্যবহার করে data-এর structure বা গঠন নির্ধারণ করা যায়। দুটিই object-এর property এবং তাদের data type নির্ধারণ করতে সাহায্য করে। দেখতে অনেকটা একই রকম হলেও এদের মধ্যে কিছু পার্থক্য রয়েছে। একজন TypeScript Developer-এর জন্য এই পার্থক্যগুলো জানা গুরুত্বপূর্ণ। 

## ২. Type কী?
TypeScript এর type ব্যবহার করে নির্দিষ্ট data type তৈরি যাই । আর এটি object, string, number, union type, tuple ইত্যাদির জন্য ব্যবহার করা যায় ।। 

### উদাহরণ:
```ts
type User = {
  name: string;
  age: number;
};

const user: User = {
  name: "Julie",
  age: 22,
};
```

## ৩. Interface কী?
interface ব্যবহার করে object-এর structure নির্ধারণ করা যাই । 

### উদাহরণ:
```ts
interface User {
  name: string;
  age: number;
}

const user: User = {
  name: "Julie",
  age: 22,
};
```

## ৪. Type এবং Interface-এর পার্থক্য

### Type
১। একই নামে নতুন করে declare করলে সাধারণত error হয়।
২। Union, Tuple ও Object তৈরি করা যায় ।
৩। & দিয়ে intersection করা যায়।

### Interface 
১। একই নামে নতুন করে declare করা যাই ।
২। 	extends দিয়ে অন্য interface extend করা যায়।
৩।  object-এর structure নির্ধারণ করা যায়

## 5. উপসংহার 
Type এবং Interface দুটিই TypeScript-এর গুরুত্বপূর্ণ অংশ। এদের মধ্যে কিছু পার্থক্য থাকলেও দুটিই code-কে পরিষ্কার, সুন্দর এবং নিরাপদ রাখতে সাহায্য করে। প্রয়োজন অনুযায়ী সঠিকটি ব্যবহার করলে code আরও সুন্দর হয়।