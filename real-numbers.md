# Die Existenz irrationaler Zahlen
## Vorbemerkung
Die Menge der rationalen Zahlen hat Lücken, eine gewisse Unvollständigkeit oder auch Diskontinuität. Auf einer Geraden gibt es unendlich viele Punkte die keiner rationalen Zahl entsprechen. Schon die alten Griechen wussten, dass die Seite eines Quadrats und seiner Diagonale nicht kommensurabel sind, d.h., man kann sie nicht mit gleichem Maß messen, wie der folgende geometrische Beweis zeigt.

![FRACT1](./2_proof.png)

1) Nach pythagoreischer Formel ist $a=\sqrt{2}b$.
2) Der eingezeichnete Kreisbogen teil die Diagonale in zwei Teilstrecken der Länge $b$ und $a-b$.
3) Das kleinere Quadrat mit der Seitenlänge $a-b$ hat eine Diagonal der Länge $\sqrt{2(a-b)^2}=\sqrt{2}(a-b)=\sqrt{2}(\sqrt{2}b-b)=2b-\sqrt{2}b=2b-a$.

Wir behaupten nun $\sqrt{2}=\frac{a}{b}$ ist kommensurabel, und damit eine rationale Zahl. Kommensurabilität bedeutet veranschaulicht:

![FRACT1](./3_commensurable.png)

$\frac{a}{b}=\frac{mc}{nc}=$, $m$ und $n$ ganze Zahlen und wir dürfen annehmen, dass $c$ das kleinste gemeinsame Vielfache ist und somit $b$ minimal.

Konstruktionsschritt 3) zeigt, dass $\sqrt{2}$ auch als $\frac{2b-a}{a-b}$ ausgedrückt werden kann. Das widerspricht jedoch der Annahme, dass $b$ minimal ist, denn $a-b < b$. Es gibt also kein kleinstes Maß $c$ für $\sqrt{2}$. Somit ist $\sqrt{2}$ nicht kommensurabel also keine rationale Zahl.

Als Ergänzung geben wir hier noch einen algebraischen Beweis für diese Tatsache an. Wieder behaupten wir, dass $\sqrt{2}$ eine Bruchzahl $\frac{a}{b}$ ist und nicht weiter gekürzt werden kann.
$$\sqrt{2}=\frac{a}{b}$$
$$2=\frac{a^2}{b^2}$$
$$2a^2=b^2$$ $a^2$ ist gerade und somit auch $a$ gerade. $a$ dürfen wir daher fortan als $2k$ schreiben.
$$2b^2=(2k)^2=4k^2$$ $2b^2$ ist damit ein Vielfaches von 4 und daher q ebenfalls gerade.

Das steht im Widerspruch zur Aussage vom Anfang, dass $\frac{a}{b}$ nicht weiter kürzbar ist. Wir haben also gezeigt, dass $\sqrt{2}$ nicht als Bruch dargestellt werden kann und damit auch keine rationale Zahl ist.

## Motivation

Die Arithmetik soll aus sich selbst heraus entwickelt werden. So lassen sich die Rechengesetze für negative und rationale Zahlen auf die Gesetze der positiven ganzen Zahlen zurückführen. Die irrationalen Zahlen müssen folglich einzig und alleine mit Hilfe der Rechengesetze für die rationalen Zahlen definiert werden. Aber wie? Hierzu muss die Frage beantwortet werden was man unter Kontinuität versteht.

Essenz von Kontinuität: Wenn alle Punkte einer Geraden in zwei Klassen fallen, sodass jeder Punkt der ersten Klasse sich auf der linken Seite befindet von jedem Punkt aus der zweiten Klasse, dann existiert ein und genau ein Punkt, der diese Unterteilung erzeugt.

## Dedekind Schnitt

Ein Dedekind Schnitt wird angegeben mit $\alpha = (A_1,A_2)$, $A_1$ und $A_2$ egeben zusammen die rationalen Zahlen, wobei jede Zahl $a_1$ in $A_1$ kleiner ist als jede Zahl $a_2$ in $A_2$. Dieses $\alpha$ unterteilt dann die Menge der rationalen Zahlen in die zwei Klassen $A_1$ und $A_2$. Ist $\alpha$ eine rationale Zahl, so ist es entweder die größte Zahl von $A_1$ oder die kleinste Zahl von $A_2$. Die Zuordnung Schnitt $\alpha$ zu einer rationalen Zahl ist eindeutig.

## Beweis der Existenz irrationaler Zahlen mit Dedekind Schnitten

Die rationalen Zahlen und die irrationalen Zahlen bilden zusammen die reellen Zahlen $\Re$. Wir zeigen nun anhand eines Dedekind Schnitts, dass irrationale Zahlen existieren und somit die reelen Zahlen die gewünschte Eigenschaft der Kontinuität besitzen, die wir bei den rationalen Zahlen vermisst haben. Es gibt unendlich viele Schnitte die nicht einer rationalen Zahl zugehören wie folgendes Beispiel zeigt.

Ausgangspunkt ist der Schnitt $(A_1,A_2)$, $A_1=$\{ $a_1$ \}, $A_2=$\{ $a_2$ \} mit der Eigenschaft ${a_1^2} <= D$ und ${a_2^2} > D$. Veranschaulichung:

![FRACT1](./1_cut.png)

$D$ sei eine positive Ganzzahl die keine Quadratzahl ist. Wir können dann schreiben
$$\lambda^2 < D < (\lambda + 1)^2$$
mit $\lambda$ ebenfalls eine positive Ganzzahl. Um zu zeigen, dass der sich daraus ergebende Schnitt $\alpha = (A_1,A_2)$ keiner rationale Zahl zugeordnet werden kann, muss die Tatsache bewiesen werden, dass es keine rationale Zahl gibt, deren Quadart $D$ ist. Um das zu tun, gehen wir von der gegenteiligen Annahme aus. Wir führen positive Ganzzahlen $t$ und $u$ ein und schreiben

$$d=\frac{t}{u}$$

$$du=t$$

$$t-du=0$$

$$t^2-d^2u^2=0$$

$$t^2-Du^2=0$$

Wir dürfen dabei annehmen, $u$ ist kleinste positive Ganzzahl die diese Gleichung erfüllt. Durch Einsetzen erhalten wir

$$\lambda^2 < \frac{t^2}{u^2} < (\lambda + 1)^2$$

$$\lambda u < t < (\lambda + 1)u$$

$$0 < t - \lambda u < u$$

$$u^{'} = t - \lambda u$$

Man bemerke $u^{'} < u$. Und auf ähnliche Weise erhalten wir

$$\lambda < \frac{t}{u} < (\lambda + 1)$$

$$\lambda tu < t^2 < (\lambda + 1) tu$$

$$\frac{\lambda t}{u} < \frac{t^2}{u^2} = D < \frac{(\lambda + 1) t}{u}$$

$$0 < Du - \lambda t < t$$

$$t^{'} = Du - \lambda t$$

Nun schreiben wir aus

$$t^{'2} - Du^{'2} = (Du - \lambda t)^2 - D(t - \lambda u)^2 = D(Du^2 - t^2) + \lambda^2(t^2 - Du^2) = (\lambda^2 - D)(t^2-Du^2)=0$$

und erkennen den Widerspruch, dass $t^{'2} - Du^{'2} = 0$. Denn wir durften annehmen, dass $u$ die kleinste Zahl ist deren Quadrat multipliziert mit $D$ in eine andere Quadratzahl überführt werden kann. Jedoch ist $u^{'} < u$. Daher kann D keine Quadratzahl sein und unser Schnitt $\alpha$ keiner rationalen Zahl zuordenbar.

TODO
Die Schnitte sind dabei wie oben beschrieben einzig und allein über die rationalen Zahlen definiert. Alle Zahlen in $\Re$, seien es rationale oder irrationale Zahlen, werden durch genau einen Schnitt repräsentiert.
