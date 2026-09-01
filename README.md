# 简历中提到的项目仓库链接

## 跨操作系统的统一任务调度器

将调度核心逻辑与OS数据结构解耦，通过自研vDSO工具库实现操作系统向任务调度模块提供任务控制接口。

主仓库：[https://github.com/rosy233333/vsched2](https://github.com/rosy233333/vsched2)

适配调度器的AsyncOS版本：[https://github.com/rosy233333/async-os/tree/vdso-test](https://github.com/rosy233333/async-os/tree/vdso-test)

## 基于vDSO的进程间通信模块

使用vDSO共享代码和数据，采用双队列结构实现IPC，支持异步API。

主仓库：[https://github.com/rosy233333/vipc](https://github.com/rosy233333/vipc)

共享队列实现：[https://github.com/rosy233333/vqueue](https://github.com/rosy233333/vqueue)

基于信号的协程唤醒实现：[https://github.com/rosy233333/async_notification](https://github.com/rosy233333/async_notification)

## 基于vDSO的，可跨地址空间共享数据的共享库

在共享库中提供声明共享数据的格式，并通过vDSO共享相应数据。实现了相关工具链，简化了vDSO共享库的开发、构建和内存映射流程。

[https://github.com/rosy233333/vdso_crate_template](https://github.com/rosy233333/vdso_crate_template)

## 统一线程与协程的任务管理模块

将协程与线程实现为同级的对象，实现线程和协程的统一调度API，支持协程的抢占（被抢占时变为线程）。

[https://github.com/rosy233333/project2210132-233191](https://github.com/rosy233333/project2210132-233191)

## QEMU模拟的硬件共享调度器

在学长设计的硬件基础上，我在QEMU模拟器中实现了硬件原型，并在ArceOS操作系统中实现了协程支持和网络模块异步改造。

QEMU中模拟的硬件：[https://github.com/rosy233333/qemu](https://github.com/rosy233333/qemu)

修改后的ArceOS：[https://github.com/rosy233333/arceos-ats-intc](https://github.com/rosy233333/arceos-ats-intc)
