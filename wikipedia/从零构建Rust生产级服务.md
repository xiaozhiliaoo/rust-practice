Serialize 特质

Serde

Rust 不提供运行时反射，一切都必须事先指定

过程宏

cargo install --version=0.6.0 sqlx-cli --no-default-features --features postgres

cargo check、cargo lint、cargo build

原子性引用计数指针Arc

将连接池使用web::Data 包装起来，其本质上是一个Arc 智能指针

sqlx::migrate!和sqlx-cli 执行sqlx migrate run 时使用的是同一个宏

可观测性的目标是可以回答你对环境提出的任意问题——这是重点——无须提前知道你的问题是什么。

log 包提供了5 个宏：trace、debug、info、warn 和error。

Rust 中一种常用的模式，被称为“资源获取即初始化”（RAII）。

cargo install cargo-udeps

cargo +nightly udeps

std::sync::Once std::sync::SyncOnceCell once_cell

once_cell 是 Rust 中一个非常有用的库，用于实现单次初始化的全局变量或延迟初始化的值。它提供了线程安全的机制，确保在多线程环境中变量只被初始化一次。这使得它在处理全局状态、配置加载或资源初始化时非常方
便。

std::io::sink

std::fmt::Display

tracing 是Rust 生态系统的基础包。而log 是最基本的技术，tracing 已成为现代诊断工程与插桩领域的核心。



std::convert::AsRef

std::fs

From/Into、TryFrom/TryInto

panic 被用来处理不可恢复的错误：没有预料到或没有办法恢复的故障模式。例如，机器内存耗尽或磁盘已满。

Rust 的主要错误处理机制是建立在 Result 类型。

精确的断言错误：claim

match 派上用场的地方：我们告诉编译器在Ok 和Err 的情况下该怎么做。

问号 ？ 语法糖： 它允许在出现故障时使用一个字符而不是多行代码块提前返回。? 会触发使用 Err 变体的提前返回，因此只能在返回Result 的函数中使用。

fake 提供了基本数据类型（整数、浮点数、字符串）和高级对象（IP 地址、国家代码等）的生成逻辑，尤其是电子邮件。
 
TryFrom Rust 的预导库 TryInto
![image](https://github.com/user-attachments/assets/2c1cced8-c37e-4bf6-9465-566229a13676)
