## Terraform Components and Bootstrap

This is my (and maybe also others eventually) try to create some lego pieces infrastructure components, that:
- do not try to be all-encompassing
- solve opinionated small problems
- still easily reusable
- are not just wrapping infra differently and make it even harder to understand
- small enough to modify, copy, clone, migrate to, away and integrate or use as bootstrap
- modules do not use other modules
- specifically modules no not generally depend on other modules so you can easily swap them out, integrate them and use them in your terraform

**this is important**: If the module does not simplify, combine or greatly improve upon using the terraform resource, we should not have a module as the only thing you'll gain is indirection, more errors, harder to upgrade and effectively less flexibility. modules can be pieces that are annoying otherwise or standardize something. If you think I have violated this rule here anywhere, let's discuss and it will be remediated. No one gains by abstracting a resource by just keeping all the complexity of it. That is so much work for nothing gained and I see this a lot. This is not your precious phone you have to wrap in casing and screen protection because otherwise the terraform resource gets scratched. 

Furthermore there will be some opinionated bootstrap repositories using them in different ways.

As usual, there isn't the one right way, but many that can work out. The important thing is that you try to structure it all - that already makes all the difference. No structure is ever perfect, but merely a tradeoff.

It is still all in its very early stages and while I have written tons of closed source code, I am rather new to this OSS thing, so please be patient on me finding the ropes.

If you wish to help, please let's chat! :) Or just open PR/Issues if you prefer 😀

Registry: https://registry.terraform.io/namespaces/terraform-components

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
