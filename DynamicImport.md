## Dynamic Import

---

**Dynamic Imports:** Unlike standard import modules, dynamic import modules are flexible in terms of when and how they are loaded. Instead of being forced to upload a module file during reading, a powerful import can be requested during use. With code separating the module into a separate batch file it can be downloaded separately **_which reduces the load on the first page._**

---

Dynamic importing is a powerful tool, and we can use it in many different scenarios to achieve better performance. It should not be overused, though, because every new import statement can lead to additional HTTPS requests.

Still, when dealing with heavy components or libraries that work in the Browser, we can depend on it to improve the bundles’ sizes and loading time.

---

## NextJs VS NodeJs?

- Next.js offers dynamic import of react components with the help of the next/dynamic

- Also, the framework allows us to import libraries and their modules dynamically

- We can think of dynamic imports as another way to split our code into manageable chunks

- We should not overuse the technique because many import statements can lead to many HTTPS requests.

- We can use dynamic imports to improve the application’s performance and make it better optimized for SEO

- **_So the best practice to use dynamic import for the non-recursive component that is at the beginning of the page._**

---

Instead of a few larger files, you end up with many smaller files instead. The downside is many smaller files means potentially many more requests.

If your Web server is serving files using HTTP/1 browsers are limited to around 6 requests at a time. Any more requests than that will be forced to wait in a queue resulting in blocked pages and speed bottlenecks.

If your server is using HTTP/2 you will see the benefit of code splitting up until a certain limit and dependent on the size of the bundles themselves. The downside regardless of server protocol is slower internet connections will just see a slow application.

---

### References

1. [Article 1](https://buhalbu.com/stream/next-js-dynamic-import-the-definitive-guide-on-how-to-use-it-for-better-app-performance)

2. [Discusstion & comments](https://www.quora.com/What-are-the-cons-of-dynamic-imports-a-k-a-code-splitting-JavaScript-files)

3. [NesxtJs Wesite](https://nextjs.org/docs/advanced-features/dynamic-import)

---
