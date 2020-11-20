# [React](https://reactjs.org/) &middot; [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/facebook/react/blob/master/LICENSE) [![npm version](https://img.shields.io/npm/v/react.svg?style=flat)](https://www.npmjs.com/package/react) [![CircleCI Status](https://circleci.com/gh/facebook/react.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/facebook/react) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://reactjs.org/docs/how-to-contribute.html#your-first-pull-request)

React is a JavaScript library for building user interfaces. (React 是一个用于构建用户界面的 JavaScript 库。)

* **Declarative:** React makes it painless to create interactive UIs. Design simple views for each state in your application, and React will efficiently update and render just the right components when your data changes. Declarative views make your code more predictable, simpler to understand, and easier to debug. (声明式：React 使创建交互式UI变的很轻松。为应用中的每个状态设计简单的视图，当数据变更时，React将有效的更新和呈现正确的组件。声明式视图使你的代码更加可预测，更易于理解且易于调试。)
* **Component-Based:** Build encapsulated components that manage their own state, then compose them to make complex UIs. Since component logic is written in JavaScript instead of templates, you can easily pass rich data through your app and keep state out of the DOM. (组件化：构建封装管理其自身状态的组件，然后把它组合成复杂的UI。 由于组件逻辑是用JavaScript而不是模板编写的，因此你可以轻松地通过app传递丰富的数据并将状态保持在DOM之外。)
* **Learn Once, Write Anywhere:** We don't make assumptions about the rest of your technology stack, so you can develop new features in React without rewriting existing code. React can also render on the server using Node and power mobile apps using [React Native](https://reactnative.dev/). (一次学习，随处编写：我们不对你的其余技术堆栈做任何假设，因此您可以在React中开发新功能而无需重写现有代码。 React还可以使用Node在服务器上进行渲染，并使用 [React Native](https://reactnative.dev/) 来支持移动应用。)

[Learn how to use React in your own project](https://reactjs.org/docs/getting-started.html). ([学习怎么在你的项目中使用React](https://zh-hans.reactjs.org/docs/getting-started.html)。)

## Installation 介绍

React has been designed for gradual adoption from the start, and **you can use as little or as much React as you need**: (React 从一开始就被设计为逐步采用，并且**你可以根据需要选择性地使用 React**)

* Use [Online Playgrounds](https://reactjs.org/docs/getting-started.html#online-playgrounds) to get a taste of React. (使用[在线体验](https://zh-hans.reactjs.org/docs/getting-started.html#online-playgrounds)来体验一下 React。)
* [Add React to a Website](https://reactjs.org/docs/add-react-to-a-website.html) as a `<script>` tag in one minute. (一分钟内使用 `<script>` 标签 [在网站中添加 React](https://zh-hans.reactjs.org/docs/add-react-to-a-website.html)。)
* [Create a New React App](https://reactjs.org/docs/create-a-new-react-app.html) if you're looking for a powerful JavaScript toolchain. (如果你正在寻找一个强大的 JavaScript 工具链来 [创建新的 React 应用](https://zh-hans.reactjs.org/docs/create-a-new-react-app.html)。)

You can use React as a `<script>` tag from a [CDN](https://reactjs.org/docs/cdn-links.html), or as a `react` package on [npm](https://www.npmjs.com/package/react). (使用 React，你可以通过 [CDN](https://zh-hans.reactjs.org/docs/cdn-links.html) 作为`<script>` 标签，也可以用 [npm](https://www.npmjs.com/package/react) 上的 `react` 包。)

## Documentation 文档

You can find the React documentation [on the website](https://reactjs.org/docs). (你可以[在网站](https://zh-hans.reactjs.org/docs)上找到React文档。)

Check out the [Getting Started](https://reactjs.org/docs/getting-started.html) page for a quick overview. (切换到[开始](https://zh-hans.reactjs.org/docs/getting-started.html)页面快速预览。)

The documentation is divided into several sections: (该文档分为几个部分：)

* [Tutorial](https://reactjs.org/tutorial/tutorial.html) ([教程](https://zh-hans.reactjs.org/tutorial/tutorial.html))
* [Main Concepts](https://reactjs.org/docs/hello-world.html) ([核心概念](https://zh-hans.reactjs.org/docs/hello-world.html))
* [Advanced Guides](https://reactjs.org/docs/jsx-in-depth.html) ([进阶指南](https://zh-hans.reactjs.org/docs/jsx-in-depth.html))
* [API Reference](https://reactjs.org/docs/react-api.html) ([API 参考](https://zh-hans.reactjs.org/docs/react-api.html))
* [Where to Get Support](https://reactjs.org/community/support.html) ([技术支持](https://zh-hans.reactjs.org/community/support.html))
* [Contributing Guide](https://reactjs.org/docs/how-to-contribute.html) ([贡献指南](https://zh-hans.reactjs.org/tutorial/how-to-contribute.html))

You can improve it by sending pull requests to [this repository](https://github.com/reactjs/reactjs.org). 你可以通过向 [此仓库] (https://github.com/reactjs/reactjs.org) 发起 `pull requests` 来改进它。

## Examples 案例

We have several examples [on the website](https://reactjs.org/). Here is the first one to get you started: (我们在[网站上](https://zh-hans.reactjs.org/)有几个示例。 这是让您入门的第一个：)

```jsx
function HelloMessage({ name }) {
  return <div>Hello {name}</div>;
}

ReactDOM.render(
  <HelloMessage name="Taylor" />,
  document.getElementById('container')
);
```

This example will render "Hello Taylor" into a container on the page. (本示例将"Hello Taylor"显示到页面的容器中)

You'll notice that we used an HTML-like syntax; [we call it JSX](https://reactjs.org/docs/introducing-jsx.html). JSX is not required to use React, but it makes code more readable, and writing it feels like writing HTML. If you're using React as a `<script>` tag, read [this section](https://reactjs.org/docs/add-react-to-a-website.html#optional-try-react-with-jsx) on integrating JSX; otherwise, the [recommended JavaScript toolchains](https://reactjs.org/docs/create-a-new-react-app.html) handle it automatically. (你会注意到我们是用来类似HTML的预发。[我们称它为JSX](https://zh-hans.reactjs.org/docs/introducing-jsx.html)。JSX并不是使用React所必须的，但它使代码更具可读性，且编写代码就像编写HTML。如果您使用React作为`<script>`标签，情阅读 [本节](https://zh-hans.reactjs.org/docs/add-react-to-a-website.html#optional-try-react-with-jsx)集成JSX；否则，[推荐的JavaScript工具链](https://zh-hans.reactjs.org/docs/create-a-new-react-app.html)会自动处理它)

## Contributing 参与贡献

The main purpose of this repository is to continue evolving React core, making it faster and easier to use. Development of React happens in the open on GitHub, and we are grateful to the community for contributing bugfixes and improvements. Read below to learn how you can take part in improving React. (这个存储库的主要目的是继续发展React核心，使其变得更快，更容易使用。 React的开发是在GitHub上进行的，我们感谢社区为bug修复和改进做出的贡献。 阅读以下内容，了解如何参与改进React。)

### [Code of Conduct](https://code.fb.com/codeofconduct) 行为规范

Facebook has adopted a Code of Conduct that we expect project participants to adhere to. Please read [the full text](https://code.fb.com/codeofconduct) so that you can understand what actions will and will not be tolerated. (Facebook 将参与者公约作为行为规范，我们希望参与项目的各位严格遵守。请阅读[全文](https://code.fb.com/codeofconduct)去了解什么行为允许，什么行为不允许。)

### [Contributing Guide](https://reactjs.org/contributing/how-to-contribute.html) 贡献指南

Read our [contributing guide](https://reactjs.org/contributing/how-to-contribute.html) to learn about our development process, how to propose bugfixes and improvements, and how to build and test your changes to React. (阅读我们的[贡献指南](https://zh-hans.reactjs.org/contributing/how-to-contribute.html)，以了解我们的开发流程，如何提出bugfixes和改进，以及如何构建和测试对React的更改。)

### Good First Issues 好的第一次 Issues

To help you get your feet wet and get you familiar with our contribution process, we have a list of [good first issues](https://github.com/facebook/react/labels/good%20first%20issue) that contain bugs which have a relatively limited scope. This is a great place to get started. (为了帮助你熟悉我们的贡献流程，我们列出来包含bug的 [好的第一次 Issues](https://github.com/facebook/react/labels/good%20first%20issue)，这是一个入门的好地方。)

### License

React is [MIT licensed](./LICENSE).
