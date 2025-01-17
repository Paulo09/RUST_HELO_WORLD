
Para criar um programa "Hello, World!" em Rust, siga os passos abaixo:

Passo a Passo
Instalar Rust

Se você ainda não tem o Rust instalado, pode instalá-lo usando o rustup, o instalador oficial do Rust. Execute o seguinte comando no terminal:

bash
Copiar código
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
Siga as instruções na tela para completar a instalação. Depois, adicione a pasta onde o Rust foi instalado ao PATH conforme as instruções fornecidas.

Criar um Novo Projeto Rust

Use o comando cargo para criar um novo projeto Rust. cargo é o sistema de build e gerenciador de pacotes do Rust.

bash
Copiar código
cargo new hello_world
cd hello_world
Escrever o Código "Hello, World!"

O Cargo cria uma estrutura básica de diretórios para você. O arquivo principal do seu projeto está em src/main.rs. Abra esse arquivo no seu editor de texto favorito e substitua o conteúdo com o seguinte código:

rust
Copiar código
fn main() {
    println!("Hello, world!");
}
Compilar e Executar

De volta ao terminal, no diretório raiz do seu projeto (onde o arquivo Cargo.toml está localizado), compile e execute seu programa com os seguintes comandos:

bash
Copiar código
cargo build
cargo run
Alternativamente, você pode usar apenas cargo run, que compilará e executará o programa em um único comando:

bash
Copiar código
cargo run
Você deve ver a seguinte saída:

Copiar código
Hello, world!
Estrutura do Projeto
Depois de criar o projeto, sua estrutura de diretórios deve ser semelhante a esta:

plaintext
Copiar código
hello_world/
├── Cargo.toml
└── src/
    └── main.rs
Cargo.toml é o arquivo de configuração do Cargo onde você especifica as dependências e outras configurações do projeto.
src/main.rs é o arquivo de código-fonte principal do seu projeto.
Explicação do Código
rust
Copiar código
fn main() {
    println!("Hello, world!");
}
fn main() { ... }: Define a função principal do programa. Em Rust, a execução do programa começa na função main.
println!("Hello, world!");: Esta linha imprime a string "Hello, world!" no console. println! é uma macro que imprime texto na saída padrão.
Agora você tem um programa "Hello, World!" funcionando em Rust. Esse é um ótimo ponto de partida para explorar mais sobre a linguagem e suas funcionalidades.
