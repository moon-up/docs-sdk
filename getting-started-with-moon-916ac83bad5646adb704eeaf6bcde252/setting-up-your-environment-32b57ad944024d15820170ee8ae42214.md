# Setting up your environment

Setting up Moon is as simple as running a few commands!

Create a new project with **Moon Create** or add Moon to an existing project.

## Create a New Project with Moon Create

Moon Create guides users through the process of establishing a tailored React & Next.JS boilerplate.

1.  Create the Next.JS and React boilerplate using create moonup in the desired directory:

    \
    **To create the boilerplate:**

{% tabs %}
{% tab title="npx" %}
```bash
npx @moonup/create
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn create @moonup
```
{% endtab %}
{% endtabs %}



1. Answer the questions in the terminal to tailor the boilerplate to the project’s needs. Once finished, Moon Create will generate the boilerplate in the desired directory:

```bash
? What is your project named? » ‘define project name here’

? Would you like to use TypeScript? » Yes/No

? Would you like to use ESLint? » Yes/No

? Would you like to use PWA? » Yes/No

? Would you like to use Moon Wallet? » Yes/No

? Would you like to use Tailwind CSS? » Yes/No

? Would you like to use `src/` directory? » Yes/No

? Would you like to customize the default import alias (@/*)? » Yes/No
```

## 🔌 **Add Moon to an Existing Project**

Adding Moon to an existing website, app, or dApp is as simple as **installing the MoonSDK**:

**To install the SDK:**



{% tabs %}
{% tab title="npm" %}
```bash
npm install @moonup/moon-sdk
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add @moonup/moon-sdk
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add @moonup/moon-sdk
```
{% endtab %}
{% endtabs %}

