# solagent.rs

connect any Ai agents to solana protocols in Rust.

## 📦 Installation

```bash
[dependencies]
solagent = "0.1.1"
```

## Quick Start

```rust
#[tokio::main]
async fn main() {
    let agent = solagent::core::agent::SolAgent::new();
    let balance = agent.get_balance(None).await.unwrap();
    println!("My balance: {}", balance);
}
```