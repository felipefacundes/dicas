# Tutorial em Construção

Aguarde o Upload do vídeo tutorial para o YouTube.
<br></br>

Enquanto não é feito o Upload do vídeo, veja o **Gif** para ter uma **noção** de como **instalar** o **Jogo** desejado (ou software do Windows). **LEMBRANDO QUE ESSE GIF É MERAMENTE EXEMPLIFICATIVO.** OU SEJA, SERVE PRA TUDO QUE HÁ NO PlayOnGit. **É SÓ ADAPTAR O CONCEITO.**

![Tuto install](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/TuToinst.gif)

**Viu como é fácil**. Basta copiar a linha inteira do comando e colar no **terminal**: dê ENTER, e pronto. Jogo instalado, pronto para uso: direto no menu iniciar > jogos.

<br></br>
**Caso precise** instalar o jogo do seu HD, porque já o possui, e não quer baixá-lo novamente. Basta, ir no **PlayOnGit** na parte:

###### "Opcional para quem quiser fazer alterações"

Copie o comando: **xdg-open ~/.jogos/scripts/run/...** referente ao seu jogo. E faça às alterações do caminho do instalador e do executável para instalar. Saiba, que o script é alto explicativo, é FÁCIL. Após instalar, **altere novamente**, e dessa vez, coloque o caminho do executável, já instalado. **NÃO esqueça de SALVAR (Ctrl + s)**. Veja esse outro **Gif** a seguir, olha que fácil:

![Tuto install manual](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/TuToinst_manual.gif)

<br></br>
Todas às instalações de Jogos do **PlayOnGit** mostrará a opção de habilitar o **Desktop Virtual**. Essa opção é importante, pois torna-se mais compatível com jogos, exemplo, GTA San Andreas, só roda em Desktop Virtual. Sem dizer que, habilitar essa opção facilita ao fechar os seus jogos com o atalho de teclado: Alt + F4, tornando extremamente eficiente à sua jogabilidade. Então, sempre vale a pena habilitar essa opção, na **Guia Gráficos** como demontrado no Gif abaixo.
![Desktop Virtual](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/Desktop_Virtual.gif)

**Caso queira apagar o menu "Wine" do seu "menu iniciar"** FAÇA O SEGUINTE:

```
rm -rf ~/.local/share/applications/*wine*
```

**Para matar o processo de um jogo ou software do Windows** EXECUTE O SEGUINTE COMANDO:

```
bash -c "pkill -9 .exe; pkill -9 wine; pkill -9 wineserver"
```
