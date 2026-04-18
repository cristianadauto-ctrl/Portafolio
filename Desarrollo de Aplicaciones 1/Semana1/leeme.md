# 📂 Portafolio de Evidencias - Semana 01
**Curso:** Desarrollo de Aplicaciones I  
**Tema:** Gestión de Proyectos con Apache Maven  

---

## 👕 Proyecto 01: Oferta de Camisas (7% + 7%)

### 📝 1. Enunciado
Diseñar un programa que determine el importe de la compra, el primer descuento (7%), el segundo descuento (7% sobre el saldo), el descuento total y el importe final a pagar por la compra de camisas.

### 📊 2. Diagrama de Clases
| Clase | Atributos | Métodos |
| :--- | :--- | :--- |
| `TiendaCamisas` | `precio`, `cantidad` | `main(String[] args)` |

> ![Diagrama](img/diagrama1.png)  
> *Nota: Representación lógica de la estructura del programa.*

### 🎨 3. Diseño de la Aplicación
A continuación, se muestra la ejecución del programa en consola con los cálculos automatizados:
![Captura de Consola](img/diseño1.png)

### 💻 4. Código de la Aplicación (Java)
```java
public class TiendaCamisas {
    public static void main(String[] args) {
        double precio = 50.0; 
        int cantidad = 5;
        double importe = precio * cantidad;
        
        double d1 = importe * 0.07;
        double d2 = (importe - d1) * 0.07;
        double dTotal = d1 + d2;
        double neto = importe - dTotal;

        System.out.printf("Importe Compra : S/. %.2f %n", importe);
        System.out.printf("Monto a Pagar  : S/. %.2f %n", neto);
    }
}
