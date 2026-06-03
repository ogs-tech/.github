# Agent AI — Explanation

> *Understanding-oriented.* Why the AI core is built this way.

## Serverless backend + mobile front-end

Agent AI pairs an **AWS Lambda** (Serverless Framework) backend with a **mobile-first** front-end
(React + Ionic + Capacitor). Capacitor lets the same React codebase ship to the web and to native
mobile, while Lambda keeps the AI backend pay-per-use with no servers to operate — a good fit for
a pro-bono / niche product like Royale IQ where load is spiky and cost discipline matters.

## Why LangGraph

The agent logic is built on **LangGraph**, which models the AI workflow as a graph of steps
(profile retrieval → deck analysis → coaching). This makes the reasoning flow explicit and
extensible — new analysis steps are added as nodes rather than tangled into one prompt.

## Shared contracts

A shared TypeScript package defines the contracts between front-end and backend, so the mobile app
and the Lambda functions stay in sync without a hand-maintained API spec.

## The engine → product path

Agent AI is the **engine**; **Royale IQ** is the productized form distributed (pro bono) by
[OGS Studio](../../../studio/royale-iq/), in the influencers niche. The engine is intended to power
future AI products beyond Royale IQ. See [How it connects](../../../explanation/how-it-connects.md).
