# Rust, Axum, PostgreSQL, and Tokio

Axum is a web framework built with Tokio, Hyper, and Tower.

git config 
git clone
git rebase -i 
git init
git add
git branch
git checkout
git fetch 
git merge 
git log 
git clean
git commit 

git add
git add
git add
git add
git add


git pull
git remote add origin-push
git push -f https://github.com/kofik/blog main

sudo systemctl start postgresql

Login using psql
sudo -u postgres psql postgres

CREATE ROLE myuser LOGIN PASSWORD 'mypass';
CREATE DATABASE mydb WITH OWNER = myuser;
\q

Login with the new user and type in your password when prompted with db password "mypass".
psql -h localhost -d mydb -U myuser

Create a table that will store our blog posts.
CREATE TABLE myposts(
post_id SERIAL PRIMARY KEY,
post_date DATE NOT NULL DEFAULT CURRENT_DATE,
post_title TEXT,
post_body TEXT);

cargo run --bin markd "My post's title" ./post.md

To insert your markdown into the database with this command
cargo run --bin markd "Some title" ./post.md
cargo run --bin blog
cargo watch -q -c -w src/ -x "run"

ls -lh blog-rs

cargo build --release 

Optimized binary in 
target/release/blog

ghostwriter 
sudo add-apt-repository ppa:wereturtle/ppa
sudo apt update
sudo apt install ghostwriter
https://ghostwriter.kde.org/it/documentation/#introduzione



Askama implements a template rendering engine based on Jinja. It generates Rust code from your templates at compile time based on a user-defined struct to hold the template's context.
https://djc.github.io/askama/

Tokio 
https://docs.rs/tokio/latest/tokio/

Tower
Tower is a library of modular and reusable components for building robust networking clients and servers.
https://docs.rs/tower/latest/tower/

tower-http is a library that provides HTTP-specific middleware and utilities built on top of tower.

Hyper is a fast and correct low-level HTTP implementation.
A protective and efficient HTTP library for all.
https://crates.io/crates/hyper


Axum
https://docs.rs/axum/latest/axum/

The Rust Performance Book
https://nnethercote.github.io/perf-book/introduction.html

UPX - the Ultimate Packer for eXecutables 
https://github.com/upx/upx


