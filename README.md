<div align="center">

# Artem Dovhyi

### Senior Software & AI Product Engineer

**Web products · LLM features · AI evaluation**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-artem--dovhyi-0A66C2?style=for-the-badge)](https://www.linkedin.com/in/artem-dovhyi)
[![Website](https://img.shields.io/badge/Website-temorix.com-111111?style=for-the-badge)](https://temorix.com)
[![Email](https://img.shields.io/badge/Email-artem%40temorix.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:artem@temorix.com)

![Remote · UTC+7](https://img.shields.io/badge/Remote-UTC%2B7-555555?style=flat-square)
![APAC, EU and US East overlap](https://img.shields.io/badge/Overlap-APAC%20·%20EU%20·%20US%20East-555555?style=flat-square)

</div>

---

I build the user-facing side of LLM features and the evaluation that shows they still work after the next change. The regression runner I built for AI assistants was adopted by six teams in about three months.

## 🧪 Featured work: a regression runner for AI assistants

AI assistant teams on an enterprise financial product couldn't tell whether a change had made their assistant worse across a real conversation. I designed and built the check they adopted.

```mermaid
flowchart LR
  QA["QA expectations<br/>in plain language"] --> R["Regression runner"]
  R <-->|"multi-turn conversation"| A["AI assistant<br/>via the product API"]
  S["Simulated user"] -->|"answers clarifying questions"| R
  R --> J["LLM judge"]
  J --> Rep["Report:<br/>verdict, cost, latency"]
```

- **The real product, not a prompt check.** The runner holds the whole conversation through the product's own API.
- **A simulated user** answers the assistant's clarifying questions, so the test reaches the answer.
- **An LLM judge** on AWS Bedrock scores the result against what QA expects.
- **Cost and latency on every run**, because every test is itself a set of LLM calls.
- **One engine, many teams.** Each assistant team keeps its own test suite.

<div align="center">

| **6** | **about 3 months** | **about 90%** |
| :---: | :---: | :---: |
| AI assistant teams adopted it | from first implementation to adoption | agreement between the judge and QA review |

</div>

A QA engineer on my team saw the need. I took it from a proof of concept to the shared tool, and the technical implementation is mine.

## 🧱 Before that

5+ years of production React and TypeScript. On an enterprise advertising platform I created the shared UI library that four modules adopted, and covered the frontend lead role for four months across three subteams.

## 🛠️ Toolbox

**AI and LLM:** LLM evaluation · LLM-as-judge · multi-turn conversation testing · simulated users · cost, token and latency tracking · AI assistant UIs

![AWS Bedrock](https://img.shields.io/badge/AWS%20Bedrock-232F3E?style=flat-square)
![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=claude&logoColor=white)
![Amazon Nova](https://img.shields.io/badge/Amazon%20Nova-232F3E?style=flat-square)

**Frontend**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Query](https://img.shields.io/badge/React%20Query-FF4154?style=flat-square&logo=reactquery&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-443E38?style=flat-square)
![Jotai](https://img.shields.io/badge/Jotai-111111?style=flat-square)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square)

**Tooling and delivery**

![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![AWS ECR](https://img.shields.io/badge/AWS%20ECR-232F3E?style=flat-square)
![VS Code extensions](https://img.shields.io/badge/VS%20Code%20extensions-007ACC?style=flat-square)

**Quality**

![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Testing Library](https://img.shields.io/badge/Testing%20Library-E33332?style=flat-square&logo=testinglibrary&logoColor=white)
![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=flat-square&logo=storybook&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white)

## 🤝 Work with me

I'm looking for contract work with product teams shipping LLM features.

- 🌏 Remote, UTC+7. Live overlap with Sydney morning, EU afternoon, and US East late morning.
- 🧾 Contracting through Temorix LLC, a US company. USD invoicing, B2B contract.
- 📬 [artem@temorix.com](mailto:artem@temorix.com) · [LinkedIn](https://www.linkedin.com/in/artem-dovhyi) · [temorix.com](https://temorix.com)
