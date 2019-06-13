# Введение в современную архитектуру Intel (IA-32) 

**Преподаватель**: Горячий Максим Сергеевич

**Дата проведения**: осенний семестр 2019 года

**Формат проведения**: 

Курс "Введение в современную архитектуру Intel (IA-32)" проходит в три этапа.
1. Две открытые лекции -- приходят все желающие
1. Рубежный контроль и отбор на спецкурс
1. Спецкурс: проведение 10-12 практических занятий.

В курсе будут рассмотрены современные возможности архитектуры **IA-32**. 
Слушателям необходимо **до начала занятий** самостоятельно изучить главы **1.2, 2.1-2.4, 3** из книги [1]

На две открытые лекции будут допущены все желающие. Каждый студент должен решить насколько ему интересна тема и "потянет" ли он спецкурс. После двух открытых лекций будет рубежный контроль. Студенты успешно его сдавшие будут допущены до спецкурса. 

## Содержание курса

1. Обзор архитектуры IA-32/32e. 
Регистры и память. 
Регистры общего назначения;
регистры x87, MMX, SSE, AVX, AVX-2, AVX-512; 
сегментные регистры; 
моделезависимые регистры (MSRs).
Модель памяти;
адресное пространство ввода-вывода (I/O);
configuration spaces.
1. Система команд. 
Команды общего назначения,
команды математического сопроцессора, 
MMX, SSE, AVX, AVX-2, AVX-512. 
Команды передачи управления.
Специализированные команды.
1. Обзор UEFI. 
Стадии загрузки. 
PEI и DXE драйверы. 
EDK2.
1. Режимы работы. Реальный режим (Real Mode), защищённый режим (Protected Mode). 
Virtual-8086. 
System Management Mode. 
IA32e (Long Mode, режим совместимости).
1. Поддержка многозадачности.
1. Защищённый режим. Уровни привилегий. Сегментные дескрипторы.
Сегментные регистры (CS, SS, DS, ES, FS, GS). GDT. LDT.
Плоская модель памяти. 
Сегментация в Long Mode.
1.  Передача управления.
Call Gates.
SYSCALL.
SYSENTER.
Автоматическое приключение стека. TSS. Task Gates.
1. Прерывания и исключения.
Аппаратные и программные прерывания.
Приоритет прерываний. 
APIC. Local APIC. 
Поддержка многопроцессорности.
1. Paging. 
Структуры PDE, PTE. TLB. PAE. PDPE. IA-32e (PLM4E). 
Механизмы обеспечения безопасности: NX bit, SMAP, SMEP.
1. Кеш. 
UC, WC, WP, WT, WB типы памяти. 
MTRRs. PAT.
1. Поддержка аппаратной виртуализации (Intel-VTx). 
VMX Root Mode, Guest Mode. 
Virtual Machine Control Structure.
VMLAUNCH, VMRESUME, VMEXIT.
Shadow Page Tables.
Extended (Nested) Page Tables. TLB Management with Virtualization.
1. Обзор расширений для защиты данных. Intel SGX. Intel MPX.
1. Режим System Management Mode.

## Список литературы

[1] Зубков С.В. Ассемблер для DOS, Windows и UNIX. ДМК Пресс, 2000.

[2] Intel R 64 and ia-32 architectures software developer’s manual volume 1: Basic architecture.

[3] Intel R 64 and ia-32 architectures software developer’s manual combined volumes 2a, 2b, 2c, and 2d: Instruction set reference, a-z.

[4] Intel R 64 and ia-32 architectures software developer’s manual combined volumes 3a, 3b, 3c, and 3d: System programming guide.

[5] Intel R 64 and ia-32 architectures software developer’s manual volume 4: Model-specific registers.

[6] Intel R 64 and ia-32 architectures optimization reference manual.

[7] Agner Fog. Software optimization resources (assembly/c++).

[8] Tom Shanley. x86 Instruction Set Architecture. MindShare Press.

[9] Tom Shanley. The Unabridged Pentium 4. MindShare Press.
