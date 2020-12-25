## Engenharia Reversa 🍚
## <br>

### 🧶 Arquitetura de processadores
Quando estamos programando em linguagens de <strong>alto nível</strong> como por exemplo javascript, não nos interessa a estrutura de um processador, justamente pelo código ser o mesmo independete da estruturação do mesmo.
<br>
No entanto, em linguagens de <strong>baixo nível</strong> como <strong>assembly</strong> o código ocorre alterações dependendo da estrutura do processador do computador.

👉 Algumas das diversas estruras de processador:
<br>
⚡ ARM
<br>
⚡ x86
<br>
⚡ x86_64

## <br>

```bash
    touch myc.c
```

- Compilando o arquivo;
```bash
    make myc
```

- Código do arquivo c:
```c
    #include <stdio.h>

    int main() {
        printf("Gabriel\n");
        return 0;
    }

```

##### 📦 Este arquivo faz a seguinte trajetória: 
##### <br>
##### A função <strong>printf()</strong> faz parte da biblioteca C (libc),
##### <br>
##### chama o kernel do sistema operacional
##### <br>
##### Assim, o kernel faz a mensagem aparecer na tela.
##### <br>
##### 👉 EXEC -> LIB -> KERNEL(syscalls(linux))
##### <br>
##### <br>
##### <br>

#### 💻 Como ver a função da biblioteca C que foi solicitada pelo arquivo executável.

```bash
    ltrace myc
```

#### 💻 Como ver a função do kernel que foi solicitada pelo arquivo executável.
```bash
    strace myc
```



