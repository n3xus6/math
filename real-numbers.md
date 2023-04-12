# Die Existenz irrationaler Zahlen
## Vorbemerkung
Die Menge der rationalen Zahlen hat Lücken, eine gewisse Unvollständigkeit oder auch Diskontinuität. Auf einer Geraden gibt es unendlich viele Punkte die keiner rationalen Zahl entsprechen. Schon die alten Griechen wussten, dass die Seite eines Quadrats und seiner Diagonale nicht kommensurabel sind, d.h., man kann sie nicht mit gleichem Maß messen, wie der folgende geometrische Beweis zeigt.

![FRACT1](./2_proof.png)

1) Nach pythagoreischer Formel ist $a=\sqrt{2}b$.
2) Der eingezeichnete Kreisbogen teil die Diagonale in zwei Teilstrecken der Länge $b$ und $a-b$.
3) Das kleinere Quadrat mit der Seitenlänge $a-b$ hat eine Diagonale der Länge $\sqrt{2(a-b)^2}=\sqrt{2}(a-b)=\sqrt{2}(\sqrt{2}b-b)=2b-\sqrt{2}b=2b-a$.

Wir behaupten nun $\sqrt{2}=\frac{a}{b}$ ist kommensurabel, und damit eine rationale Zahl. Kommensurabilität bedeutet veranschaulicht:

![FRACT1](./3_commensurable.png)

$\frac{a}{b}=\frac{mc}{nc}=$, $m$ und $n$ ganze Zahlen und wir dürfen annehmen, dass $c$ das kleinste gemeinsame Vielfache ist und somit $b$ minimal.

Konstruktionsschritt 3) zeigt, dass $\sqrt{2}$ auch als $\frac{2b-a}{a-b}$ ausgedrückt werden kann. Das widerspricht jedoch der Annahme, dass $b$ minimal ist, denn $a-b < b$. Es gibt also kein kleinstes Maß $c$ für $\sqrt{2}$. Somit ist $\sqrt{2}$ nicht kommensurabel also keine rationale Zahl.

Als Ergänzung geben wir hier noch einen algebraischen Beweis für diese Tatsache an. Wieder behaupten wir, dass $\sqrt{2}$ eine Bruchzahl $\frac{a}{b}$ ist und nicht weiter gekürzt werden kann.
$$\sqrt{2}=\frac{a}{b}$$
$$2=\frac{a^2}{b^2}$$
$$2b^2=a^2$$ $a^2$ ist gerade und somit auch $a$ gerade. $a$ dürfen wir daher fortan als $2k$ schreiben.
$$2b^2=(2k)^2=4k^2$$ $2b^2$ ist damit ein Vielfaches von 4 und daher b ebenfalls gerade.

Das steht im Widerspruch zur Aussage vom Anfang, dass $\frac{a}{b}$ nicht weiter kürzbar ist. Wir haben also gezeigt, dass $\sqrt{2}$ nicht als Bruch dargestellt werden kann und damit keine rationale Zahl ist.

## Motivation

Die Arithmetik soll aus sich selbst heraus entwickelt werden. So lassen sich die Rechengesetze für negative und rationale Zahlen auf die Gesetze der positiven ganzen Zahlen zurückführen. Die irrationalen Zahlen müssen folglich einzig und alleine mit Hilfe der Rechengesetze für die rationalen Zahlen definiert werden. Aber wie? Hierzu muss die Frage beantwortet werden was man unter Kontinuität versteht.

Essenz von Kontinuität: Wenn alle Punkte einer Geraden in zwei Klassen fallen, sodass jeder Punkt der ersten Klasse sich auf der linken Seite befindet von jedem Punkt aus der zweiten Klasse, dann existiert ein und genau ein Punkt, der diese Unterteilung erzeugt.

## Dedekind Schnitt

Ein Dedekind Schnitt $\alpha = (A_1,A_2)$ unterscheidet zwei Klassen $A_1$ und $A_2$ dadurch, dass jede Zahl $a_1$ in $A_1$ kleiner ist als jede Zahl $a_2$ in $A_2$. $a_1$ und $a_2$ sind rationale Zahlen. Es gibt genau eine Zahl $\alpha$ die einen Schnitt eindeutig bestimmt, sodass gilt $a_1 < \alpha < a_2$. Ist $\alpha$ eine rationale Zahl, kann diese entweder zu $A_1$ oder zu $A_2$ zugeordnet werden. Dann ist sie entweder die größte Zahl von $A_1$ oder die kleinste Zahl von $A_2$. Unabhängig davon betrachten wir beide Fälle als wesentlich identisch.

## Vorhaben

Die rationalen Zahlen und die irrationalen Zahlen bilden zusammen die reellen Zahlen $\Re$. Wir zeigen nun anhand eines Dedekind-Schnitts, dass irrationale Zahlen existieren. Die reelen Zahlen besitzen die gewünschte Eigenschaft der Kontinuität, die wir bei den rationalen Zahlen vermisst haben. Es gibt unendlich viele Schnitte die nicht einer rationalen Zahl zugeordnet werden können.

## Erstellen einer irrationalen Zahl

Ausgangspunkt ist der Schnitt $\alpha = (A_1,A_2)$:

$$A_1=\\{a_1\\}=\\{x|x\leq0 \lor (x>0 \land x^2\leq D)\\}$$

$$A_2=\\{a_2\\}=\\{x|x>0 \land x^2>D\\}$$

Veranschaulichung:

![FRACT1](./1_cut.png)

Mit $x$ rationale Zahl, $D$ positive ganze Zahl. $a_1 < a_2$ für alle $a_1$ und alle $a_2$.

Zu zeigen: $\alpha \notin Q$, wenn $D$ **nicht** das Quadrat einer ganzen Zahl ist. Wäre $\alpha$ eine rationale Zahl, so hätte $A_1$ eine größte Zahl oder $A_2$ eine kleinste Zahl, nämlich $\alpha$.

Erlaubt der Schnitt, dass $D$ nicht das Quadrat einer ganzen Zahl sein kann? Das hieße, $D$ befindet sich zwischen zwei Quadratzahlen

$$\lambda^2 < D < (\lambda + 1)^2, \lambda \in N$$

Wäre nun $D$ eine Quadrat einer ganzen Zahl könnte man schreiben ($t, u$ positive ganze Zahlen)

$$d=\frac{t}{u}$$

$$du=t$$

$$t-du=0$$

$$t^2-d^2u^2=0$$

$$t^2-Du^2=0$$

$u$ soll hierbei **minimal** sein. Durch Einsetzen erhält man

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

Ausformulieren zeigt

$$t^{'2} - Du^{'2} = (Du - \lambda t)^2 - D(t - \lambda u)^2 = D(Du^2 - t^2) + \lambda^2(t^2 - Du^2) = (\lambda^2 - D)(t^2-Du^2)=0$$

, wegen $(t^2-Du^2)=0$. Wir erkennen den Widerspruch zur Annahme, dass $u$ die kleinste Zahl ist deren Quadrat multipliziert mit $D$ in eine andere Quadratzahl überführt werden kann. Jedoch ist $u^{'} < u$. Daher kann D keine Quadratzahl sein und für alle $x$ gilt $x^2 < D$ oder $x^2>D$.

TODO
