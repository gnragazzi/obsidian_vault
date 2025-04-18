```
función Crear-Sentencia-Percepción(percepción, t) retorna sentencia
	entradas: percepción, una lista, [olor, brisa, brillo, golpe, grito]
			  t, un contador, indicando el tiempo
	si olor entonces sent ← Olorᵗ sino sent ← ¬ Olorᵗ
	si brisa entonces sent ← sent ∧ Brisaᵗ sino sent ← sent ∧ ¬ Brisaᵗ
	si brillo entonces sent ← sent ∧ Brilloᵗ sino sent ← sent ∧ ¬Brilloᵗ
	si golpe entonces sent ← sent ∧ Golpeᵗ sino sent ← sent ∧ ¬ Golpeᵗ
	si grito entonces sent ← sent ∧ Gritoᵗ sino sent ← sent ∧ ¬ Gritoᵗ
	retornar sent
```