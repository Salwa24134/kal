---
title: TRANFORMASI LINIER

---


## Pembuktian Transformasi Linier

#### Diberikan sebuah transformasi:

$$
T(v_1, v_2) = (v_1 + v_2, v_1)
$$

Tujuan kita adalah membuktikan bahwa $T$ merupakan **transformasi linier**.

---

### Syarat Transformasi Linier

Agar suatu transformasi $T$ dikatakan **linier**, maka untuk sembarang vektor $\mathbf{a}, \mathbf{b} \in \mathbb{R}^2$ dan skalar $c \in \mathbb{R}$, harus berlaku:

1. **Aditivitas (Penjumlahan):**

   $$
   T(\mathbf{a} + \mathbf{b}) = T(\mathbf{a}) + T(\mathbf{b})
   $$

2. **Homogenitas (Perkalian skalar):**

   $$
   T(c \cdot \mathbf{a}) = c \cdot T(\mathbf{a})
   $$

---

### Langkah Pembuktian Transformasi Linier

#### 1. Aditivitas

Misalkan:

$$
\mathbf{a} = (a_1, a_2), \quad \mathbf{b} = (b_1, b_2)
$$

Hitung:

$$
T(\mathbf{a} + \mathbf{b}) = T(a_1 + b_1, a_2 + b_2) = ((a_1 + b_1) + (a_2 + b_2), a_1 + b_1)
$$

$$
= (a_1 + a_2 + b_1 + b_2, a_1 + b_1)
$$

Sementara:

$$
T(\mathbf{a}) + T(\mathbf{b}) = (a_1 + a_2, a_1) + (b_1 + b_2, b_1) = (a_1 + a_2 + b_1 + b_2, a_1 + b_1)
$$

Jadi:

$$
T(\mathbf{a} + \mathbf{b}) = T(\mathbf{a}) + T(\mathbf{b})
$$

**Syarat aditif terpenuhi**

---

#### 2. Homogenitas

Misalkan $c \in \mathbb{R}$, dan $\mathbf{a} = (a_1, a_2)$

Hitung:

$$
T(c \cdot \mathbf{a}) = T(ca_1, ca_2) = (ca_1 + ca_2, ca_1) = c(a_1 + a_2, a_1)
$$

Sementara:

$$
c \cdot T(\mathbf{a}) = c \cdot (a_1 + a_2, a_1) = (c(a_1 + a_2), c a_1)
$$

Jadi:

$$
T(c \cdot \mathbf{a}) = c \cdot T(\mathbf{a})
$$

**Syarat homogen terpenuhi**

---

### Kesimpulan

Karena transformasi:

$$
T(v_1, v_2) = (v_1 + v_2, v_1)
$$

memenuhi kedua sifat aditif dan homogen, maka:

$$
\boxed{T \text{ adalah transformasi linier.}}
$$

---

