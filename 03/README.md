> :white_check_mark: *Jeśli będziesz mieć problem z rozwiązaniem tego zadania, poproś o pomoc na odpowiednim kanale na Slacku, tj. `s5e05-php-refactoring` (dotyczy [mentee](https://devmentor.pl/mentoring-javascript/)) lub na ogólnodostępnej i bezpłatnej [społeczności na Discordzie](https://devmentor.pl/discord). Pamiętaj, aby treść Twojego wpisu spełniała [odpowiednie kryteria](https://devmentor.pl/jak-prosic-o-pomoc/).*

&nbsp;

# `#03` PHP: Refactoring Techniques

Przygotuj klasę `Query`, która pozwoli generować kod SQL z wykorzystaniem [łąńcuchowego wywołania](https://bulldogjob.pl/readme/upiekszanie-kodu-w-php-za-pomoca-method-chaining).

Przykład:
```
$query = new Query();
$sql = $query->table('user')->where('id = :id')->get();
```

Postaraj się zaimplementować to rozwiązanie w klasie `Database`, z której do tej pory korzystałeś.

&nbsp;
> :no_entry: *Jeśli nie posiadasz materiałów do tego zadania tj. **Wideo**, znajdziesz je na stronie [laracasts.com](https://laracasts.com/referral/bogolubow)*

> :arrow_left: [*poprzednie zadanie*](./../02) | [*następne zadanie*](./../04) :arrow_right:
