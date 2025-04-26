
# Awesome AI Agent Protocols

> 🧠 Curated list of communication protocols for LLM-based AI Agents  
> Inspired by the paper: *A Survey of AI Agent Protocols* ([Yang et al., 2025](https://arxiv.org/abs/2504.16736))

---

## 🌐 Motivation & Insights

With the rise of Large Language Model (LLM) agents in areas like customer service, content creation, and healthcare, a major bottleneck has emerged: **there is no standard way for these agents to communicate with tools, resources, or each other**.

This lack of standardized communication protocols:
- Creates silos between systems.
- Limits scalability and collaboration.
- Hinders collective intelligence from emerging.

Drawing an analogy from the early days of the Internet, this fragmentation echoes the era before TCP/IP. Just as TCP/IP transformed isolated networks into a unified internet, agent protocols aim to build a **network of distributed intelligence**—enabling dynamic, secure, and cooperative AI agents.

> A unified protocol infrastructure is not just a technical fix—it’s a **paradigm shift** for building the "Internet of Agents".

---

## 🔧 Protocol Taxonomy

We follow the two-dimensional classification proposed in the paper:

| Type | General Purpose | Domain Specific |
|------|------------------|------------------|
| **Context-Oriented** | [MCP](#model-context-protocol-mcp) | [agents.json](#agentsjson) |
| **Inter-Agent** | [A2A](#agent2agent-protocol-a2a), [ANP](#agent-network-protocol-anp), [AITP](#agent-interaction--transaction-protocol-aitp), [AComP](#agent-communication-protocol-acomp), [AConP](#agent-connect-protocol-aconp), [Agora](#agora) | [LMOS](#language-model-operating-system-lmos), [Agent Protocol](#agent-protocol), [LOKA](#loka), [PXP](#pxp), [CrowdES](#crowdes), [SPPs](#spatial-population-protocols-spps) |

---

## 📘 Protocols Details

### 🧠 Context-Oriented Protocols

#### Model Context Protocol (MCP)
- **Proposer**: Anthropic (2024)
- **Goal**: Standardize resource access & tool usage by agents
- **Tech**: RPC, OAuth, HTTP Streaming
- **Link**: [MCP Whitepaper](https://www.anthropic.com/index/mcp)

#### agents.json
- **Proposer**: Wildcard AI
- **Goal**: AI-native OpenAPI extension for tool discovery and flow definition
- **Tech**: JSON at `/.well-known/agents.json`
- **Link**: [agents.json GitHub](https://github.com/wildcard-xyz/agents.json)

---

### 🤝 Inter-Agent Protocols

#### Agent2Agent Protocol (A2A)
- **Proposer**: Google
- **Goal**: Enable intra-org agent collaboration
- **Tech**: JSON-RPC, SSE, OpenAPI
- **Link**: [Google A2A](https://ai.googleblog.com/2024/12/agent-to-agent-protocol.html)

#### Agent Network Protocol (ANP)
- **Proposer**: ANP Community (Chang, 2024)
- **Goal**: Cross-domain decentralized agent interoperability
- **Tech**: JSON-LD, DID
- **Link**: [ANP GitHub](https://github.com/agent-network-protocol/anp)

#### Agent Interaction & Transaction Protocol (AITP)
- **Proposer**: NEAR Foundation
- **Goal**: Secure, decentralized agent interactions
- **Tech**: Blockchain, HTTP
- **Link**: [AITP GitHub](https://github.com/near/aitp)

#### Agent Communication Protocol (AComP)
- **Proposer**: IBM
- **Goal**: Define features for multi-agent communication
- **Tech**: OpenAPI
- **Link**: [AComP GitHub](https://github.com/ibm/agent-communication-protocol)

#### Agent Connect Protocol (AConP)
- **Proposer**: LangChain
- **Goal**: Unified agent execution interfaces
- **Tech**: OpenAPI, JSON
- **Link**: [LangChain AConP](https://spec.acp.agntcy.org/)

#### Agora
- **Proposer**: Marro et al. (2024)
- **Goal**: Meta-protocol negotiation via LLMs
- **Tech**: Protocol Generation
- **Link**: [Agora Paper](https://arxiv.org/abs/2410.11905)

---

### 🏭 Domain-Specific Protocols

#### Language Model Operating System (LMOS)
- **Proposer**: Eclipse Foundation
- **Goal**: IoT + Agent OS for interoperability
- **Tech**: JSON-LD, DID
- **Link**: [LMOS GitHub](https://eclipse.dev/lmos/)

#### Agent Protocol
- **Proposer**: AI Engineer Foundation
- **Goal**: Open control API for agents
- **Tech**: RESTful, OpenAPI
- **Link**: [Agent Protocol GitHub](https://github.com/ai-engineer-foundation/agent-protocol)

#### LOKA
- **Proposer**: Ranjan et al. (2025)
- **Goal**: Decentralized ethical agent coordination
- **Tech**: DECP, DID, VCs
- **Link**: [LOKA Paper](https://arxiv.org/abs/2504.10915)

#### PXP
- **Proposer**: Srinivasan et al. (2024)
- **Goal**: Human-LLM bi-directional interaction protocol
- **Tech**: Finite State + Blackboard
- **Link**: [PXP Paper](https://arxiv.org/abs/2410.20600)

#### CrowdES
- **Proposer**: Bae et al. (2025)
- **Goal**: Realistic robot-crowd simulation
- **Tech**: Markov Chains + Diffusion Models
- **Link**: [CrowdES Paper](https://arxiv.org/abs/2504.04756)

#### Spatial Population Protocols (SPPs)
- **Proposer**: Gąsieniec et al. (2024)
- **Goal**: Robot consensus in distributed systems
- **Tech**: Self-stabilizing coordination
- **Link**: [SPPs Paper](https://arxiv.org/abs/2411.08434)

---

## 🔍 Use Cases (from paper)

- **MCP**: Single-agent tool orchestration
- **A2A**: Enterprise multi-agent orchestration
- **ANP**: Decentralized cross-domain networks
- **Agora**: Meta-protocol generation

---

## 📚 Citation

If you find this repository helpful, please consider citing our paper:

```bibtex
@misc{yang2025surveyaiagentprotocols,
  title={A Survey of AI Agent Protocols}, 
  author={Yingxuan Yang and Huacan Chai and Yuanyi Song and Siyuan Qi and Muning Wen and Ning Li and Junwei Liao and Haoyi Hu and Jianghao Lin and Gaowei Chang and Weiwen Liu and Ying Wen and Yong Yu and Weinan Zhang},
  year={2025},
  eprint={2504.16736},
  archivePrefix={arXiv},
  primaryClass={cs.AI},
  url={https://arxiv.org/abs/2504.16736}, 
}
```


