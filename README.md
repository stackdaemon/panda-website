### Q.1 > What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

*** Ans Number #1:
### getElementById() ==> কেবলমাত্র নির্দিষ্ট id অনুযায়ী একটা মাত্র element আনে । যদি উপাদানটি বিদ্যমান না থাকে ,তবে null প্রদান করে। আর id সবসময় unique হয় ।
###  getElementsByClassName () ==> এটি নির্দিষ্ট class অনুযায়ী এক বা একাধিক element আনে। এটা একটা HTMLCollection দেয়, যেটা array-এর মতো কিন্তু পুরোপুরি array না।
### querySelector() ==> CSS selector ব্যবহার করে প্রথম যে element মিলে যায়, শুধু সেটাই আনে।
### querySelectorAll () ==> এটি querySelector মতোই তবে CSS selector ব্যবহার করে যত element মিলে যায়, সব আনে এবং NodeList আকারে দেয়।

### Q.2 >How do you create and insert a new element into the DOM?

*** Ans Number #2:
### নতুন element তৈরি জন্য document.createElement("tagName") ব্যবহার করা হয়। 
const newDiv = document.createElement("div");
### DOM এ ইনসার্ট করা → যেকোনো parent element এর মধ্যে appendChild() বা append() দিয়ে বসানো হয়।
document.body.appendChild(newDiv);
