# Lisp(Scheme)言語でソートアルゴリズムの復習

高級言語のようにfor文やwhile文が無いため、
ループ処理は基本的に再帰的に行う。

## バブルソート

|引数|役割|
|---|---|
|list|バブルソート対象のlistを格納する。最大値が評価される度に `tempList` をリセットするための引数|
|tempList|評価後の最大値が常に一番左端にある状態として処理する引数。処理途中で大なり判定の際に偽であった数値は常に除いている。また `result` に含まれる数値を大なり判定で評価しないようにしている。|
|count| `targetList` のlength回分評価させることによりバブルソートを行っている|
|result| `tempList` のlengthが1になる度にn純目の最大値を左端に加えている|
