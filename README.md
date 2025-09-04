# TCC Battlecode Engine RS
An unofficial, community-driven port of the MIT Battlecode game engine to the Rust programming language. This project aims to create a high-performance, safe, and modern version of the engine for educational and competitive use.
This port is based on the Battlecode 2025 version.
- Original Project: [battlecode/battlecode25](https://github.com/battlecode/battlecode25)
- Official Website: [battlecode.org](battlecode.org)
## About Battlecode
Battlecode is a real-time strategy (RTS) game and programming competition from MIT. Participants write an AI player in Java or Python to command a virtual robot army. The game engine runs matches between players to determine the winner.
## Project Goals
The primary goal of this project is to create a complete, functional version of the Battlecode engine in Rust. We aim to:
- **Achieve High Performance:** Leverage Rust's performance characteristics to create a fast and efficient game.
- **Ensure Safety and Reliability:** Utilize Rust's memory and thread safety guarantees to build a robust and crash-resistant server.
- **Provide a Modern Toolchain:** Use Cargo and the Rust ecosystem for a modern, easy-to-use build process.
- **Enable Multi-Language Player APIs:** The ultimate goal is to expose a clean, stable API from the Rust core, allowing competitors to write bots in a variety of languages, including:
  - **Rust**
  - **C++**
  - **Python**
  - **Java**
This project is an excellent opportunity for those interested in Game Development, systems programming, and cross-language interoperability.
## Current Status
### 🚧 This project is in the early stages of development. 🚧
The initial focus is on porting the core data structures, game constants, and the main game loop in Rust. See the [Issues](https://github.com/michaelnutt2/tccd-battlecode-engine-rs/issues) for a detailed project plan and tasks that are ready to be worked on.
## Getting Started
To build the core engine, you will need the Rust toolchain installed.
```bash
# 1. Clone the repository
git clone https://github.com/michaelnutt2/tccd-battlecode-engine-rs.git
cd tccd-battlecode-engine-rs

# 2. Build the project
cargo build --release

# 3. Run the engine (example)
# Actual command-line arguments are TBD
./target/release/tccd-battlecode-engine-rs --map "maps/default.map25" "player1" "player2"
```
## Contributing
