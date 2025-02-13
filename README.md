# @LS UI-KIT

## Описание<a name="info"></a>

Библиотека react компонентов предназначена для использования во внутренних проектах и для настольного и мобильного сайта

- [Описание](#info)
- [Структура проекта](#structure)
  - [Диаграмма зависимостей](#dependence)
- [Подходы к разработке компонентов](#usage)
- [Storybook](#credits)
- [Ссылки](#credits)
- [Тесты](#license)

## Installation

What are the steps required to install your project? Provide a step-by-step description of how to get the development environment running.

## Usage

Provide instructions and examples for use. Include screenshots as needed.

To add a screenshot, create an `assets/images` folder in your repository and upload your screenshot to it. Then, using the relative filepath, add it to your README using the following syntax:

```mermaid
graph TD;
    helpers-->basics;
    helpers-->layouts;
    helpers-->components;
    helpers-->widgets;
    helpers-->hooks;
    basics-->layouts;
    basics-->components;
    basics-->widgets;
    layouts-->components;
    layouts-->widgets;
    components-->widgets;
    hooks-->components
    hooks-->layouts
    hooks-->widgets
```

```mermaid
flowchart TB
    styles-->shared-folders
    styles-->react-folders
    shared-folders-->react-folders
    styles-->supporting-folders
    react-folders-->supporting-folders
    shared-folders-->supporting-folders
    subgraph shared-folders
    types-->constants
    constants-->types
    types-->helpers
    constants-->helpers
    end
    subgraph react-folders
    basics-->layouts
    basics-->components
    basics-->widgets
    hooks-->layouts
    hooks-->components
    hooks-->widgets
    layouts-->components
    layouts-->widgets
    components-->widgets
    end
    subgraph supporting-folders
    __tests__
    __mocks__
    stories
    end
```

```mermaid
flowchart TB
    styles-->shared-folders
    styles-->component-folders
    shared-folders-->component-folders
    styles-->supporting-folders
    component-folders-->supporting-folders
    shared-folders-->supporting-folders
    subgraph shared-folders
    types-->constants
    constants-->types
    types-->helpers
    constants-->helpers
    constants-->hooks
    helpers-->hooks
    types-->hooks
    end
    subgraph component-folders
    component-base-->component
    component-->component-panel
    component-input-->component-panel
    end
    subgraph supporting-folders
    __tests__
    __mocks__
    stories
    end
```

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

## Структура проекта<a name="structure"></a>

List your collaborators, if any, with links to their GitHub profiles.

If you used any third-party assets that require attribution, list the creators with links to their primary web presence in this section.

If you followed tutorials, include links to those here as well.
### Диаграмма зависимостей<a name="dependence"></a>
![зависимости](./structure.png)

## License

The last section of a high-quality README file is the license. This lets other developers know what they can and cannot do with your project. If you need help choosing a license, refer to [https://choosealicense.com/](https://choosealicense.com/).

---

🏆 The previous sections are the bare minimum, and your project will ultimately determine the content of this document. You might also want to consider adding the following sections.

## Badges

![badmath](https://img.shields.io/github/languages/top/lernantino/badmath)

Badges aren't necessary, per se, but they demonstrate street cred. Badges let other developers know that you know what you're doing. Check out the badges hosted by [shields.io](https://shields.io/). You may not understand what they all represent now, but you will in time.

## Features

If your project has a lot of features, list them here.

## How to Contribute

If you created an application or package and would like other developers to contribute it, you can include guidelines for how to do so. The [Contributor Covenant](https://www.contributor-covenant.org/) is an industry standard, but you can always write your own if you'd prefer.

## Tests

Go the extra mile and write tests for your application. Then p