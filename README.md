# MGSmartFlow

[![License](https://img.shields.io/badge/license-PolyForm%20Perimeter%201.0.0-5351FB)](LICENSE.md)

MGSmartFlow é um **layout customizado para Fyne** que facilita a criação de interfaces dinâmicas baseadas em **linhas e colunas**, com controle inteligente de espaçamento, redimensionamento e posicionamento de widgets.

Ele foi projetado para simplificar layouts complexos sem depender apenas dos layouts padrões do Fyne.

---

## ✨ Recursos

* 📐 Layout por **linhas** e **colunas**
* 📏 Redimensionamento automático ou fixo por widget
* 🧭 Posicionamento manual opcional
* ↔️ Espaçamento global ou individual
* 🔄 Atualização dinâmica do layout
* 🧩 Wrapper simples para uso direto

---

## 📦 Instalação

```bash
go get github.com/profmugomes/mgsmartflow
```

---

## 🚀 Uso Básico

### Criando o SmartFlow

```go
flow := mgsmartflow.New()
```

### Adicionando uma linha

```go
flow.AddRow(widget.NewLabel("Linha única"))
```

### Adicionando colunas na mesma linha

```go
flow.AddColumn(
	widget.NewButton("Botão 1", nil),
	widget.NewButton("Botão 2", nil),
)
```

---

## 📐 Controle de Layout

### Redimensionar um widget

```go
flow.Resize(btn, 120, 40)
```

### Mover manualmente um widget

```go
flow.Move(btn, 10, 20)
```

### Espaçamento individual entre widgets

```go
flow.Gap(btn, 15, 10)
```

### Espaçamento global do layout

```go
flow.GlobalGap(10, 10)
```

---

## 🧩 Compatibilidade

* Go 1.26.5+
* Fyne 2.8.0

---

## 👤 Autor

**Murilo Gomes Julio**

🔗 [https://www.profmugomes.com.br](https://www.profmugomes.com.br)

📺 [https://youtube.com/@profmugomes](https://youtube.com/@profmugomes)

---

## License

Copyright (c) 2025-2026 Murilo Gomes Julio. All Rights Reserved.

This project is licensed under the PolyForm Perimeter License 1.0.0.

### Summary

This software is available for commercial and noncommercial use, subject to the terms of the PolyForm Perimeter License 1.0.0.

You may:

* ✔ Use the software for commercial and noncommercial purposes.
* ✔ Inspect and study the source code.
* ✔ Modify the software.
* ✔ Create derivative works based on the software.
* ✔ Redistribute the software and permitted modifications.

You may not:

* ✖ Provide a product that competes with the software.

See the full license terms at LICENSE.md.

This summary is provided for convenience only and does not replace or modify the full license terms.