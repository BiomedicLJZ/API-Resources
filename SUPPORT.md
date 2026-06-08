# Support

This project is an educational resource for the Software Engineering course at CUGDL (Centro Universitario de la Ciénega, Universidad de Guadalajara).

## Getting Help

| Channel | Use for |
|---------|---------|
| [GitHub Issues](../../issues) | Bugs, incorrect code examples, broken UI |
| [GitHub Discussions](../../discussions) | Conceptual questions, archetype comparisons, suggestions |
| Course forums | Assignment-specific questions (enrolled students only) |

## FAQ

**Q: The code examples don't run when I paste them — why?**
The snippets are illustrative. They require local dependencies installed (`pip install fastapi spyne zeep grpcio`, `npm install soap`, etc.) and a running server instance. Follow the import statements shown at the top of each snippet.

**Q: Which API archetype should I use for my project?**
Use the **Quick Decision Map** on the Overview tab. The general rule: default to **REST** unless you have a specific reason not to (real-time → WebSocket/SSE, internal microservices → gRPC, external events → Webhook, legacy enterprise → SOAP).

**Q: Is SOAP still relevant to learn?**
For new projects: almost never. For integrating with existing banking systems, healthcare platforms (HL7), or government APIs: absolutely yes. Many enterprises still run SOAP services, and understanding XML envelopes + WSDL contracts is essential for enterprise software engineers.

**Q: Can I use the code examples in my own projects?**
Yes, under the [MIT License](./LICENSE). Consult `SECURITY.md` for production hardening notes before deploying any snippet.

**Q: How do I add a new API archetype to the guide?**
See `CONTRIBUTING.md` — it includes the full schema each archetype entry must follow.

## Learning Resources

| Archetype | Key Resource |
|-----------|-------------|
| REST | [restfulapi.net](https://restfulapi.net/) · [FastAPI docs](https://fastapi.tiangolo.com/) |
| GraphQL | [graphql.org/learn](https://graphql.org/learn/) · [Strawberry](https://strawberry.rocks/docs) |
| gRPC | [grpc.io/docs](https://grpc.io/docs/) · [Protocol Buffers](https://protobuf.dev/) |
| WebSocket | [MDN WebSocket API](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) |
| Webhook | [webhooks.fyi](https://webhooks.fyi/) · [Stripe guide](https://stripe.com/docs/webhooks) |
| SSE | [MDN Server-Sent Events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events) |
| SOAP | [W3C SOAP spec](https://www.w3.org/TR/soap/) · [zeep docs](https://docs.python-zeep.org/) · [spyne](http://spyne.io/docs/) |

## Maintainer

**Leonardo Juárez Zucco**
Ingeniería De Software — Centro Universitario de Guadalajara, Universidad de Guadalajara
Contact: leonardo.juarez.zucco@gmail.com
