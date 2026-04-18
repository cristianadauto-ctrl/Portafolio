# 📂 Portafolio Académico - Semana 01
**Curso:** Desarrollo de Aplicaciones I  
**Estudiante:** Cristian Adauto  
**Tecnologías:** Java (JDK 17+), Apache Maven, NetBeans

---

## 👔 Proyecto 01: Sistema de Descuentos "Verano Total" (7% + 7%)

### 📝 Enunciado
Implementar una aplicación que calcule el importe de compra para camisas aplicando un descuento sucesivo de temporada.
* **Fórmulas aplicadas:**
  * $Importe = Precio \times Cantidad$
  * $D1 = Importe \times 0.07$
  * $D2 = (Importe - D1) \times 0.07$
  * $Total = Importe - (D1 + D2)$

### 📊 Diagrama de Clases (UML)
| Clase | Atributos | Métodos |
| :--- | :--- | :--- |
| `TiendaCamisas` | `precio`, `cantidad` | `main(String[] args)` |

> [!TIP]
> **[SUBE TU CAPTURA AQUÍ]** -> `![Diagrama](img/diagrama1.png)`

### 💻 Código Fuente (Snippet)
```java
// Implementación optimizada con manejo de decimales
double desc1 = importeCompra * 0.07;
double desc2 = (importeCompra - desc1) * 0.07;
double pagoFinal = importeCompra - (desc1 + desc2);
