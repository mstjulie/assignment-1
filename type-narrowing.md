Blog 2: Type Narrowing in TypeScript 

১. ভূমিকা 
TypeScript-এ Type Narrowing একটি গুরুত্বপূর্ণ বিষয় । এর মাধ্যমে কোনো variable-এর type আরও নির্দিষ্ট করা যাই । Type Narrowing ব্যবহার করে আমরা নিরাপদে সেই data নিয়ে কাজ করতে পারি এবং code-এর error কমাতে পারি।

২. Type Narrowing কী?
Type Narrowing এর মাধ্যমে TypeScript কোনো variable-এর সম্ভাব্য type কমিয়ে আরও নির্দিষ্ট type বুঝতে পারে । 

উদাহরণ:
function processInput(value: string | number) {
  if (typeof value === "string") {
    return value.toUpperCase();
  }

  return value * 10;
}

৩. Type Narrowing-এর কিছু পদ্ধতি

# typeof ব্যবহার
function processInput(value: string | number): string | number {
  if (typeof value === "string") {
    return value.toUpperCase();
  }
  return value * 10;
}

# instanceof ব্যবহার
function getDate(value: Date | string) {
  if (value instanceof Date) {
    return value.toDateString();
  }

  return value;
}

৪. Type Narrowing কেন গুরুত্বপূর্ণ?
Type Narrowing ব্যবহার করলে

Code-এর error কমানো যায়।
সঠিক data type অনুযায়ী কাজ করা যায়।
Code আরও নিরাপদ হয়।
TypeScript-এর type checking আরও ভালোভাবে ব্যবহার করা যায়। 

৫. উপসংহার
Type Narrowing TypeScript-এর একটি গুরুত্বপূর্ণ বৈশিষ্ট্য। এটি আমাদের variable-এর সঠিক type বুঝতে সাহায্য করে। বিভিন্ন পদ্ধতি ব্যবহার করে আমরা সহজেই type narrow করতে পারি। তাই TypeScript দিয়ে নিরাপদ ও পরিষ্কার code লেখার জন্য Type Narrowing শেখা প্রয়োজন।