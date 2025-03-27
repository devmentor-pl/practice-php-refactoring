> :white_check_mark: *Jeśli będziesz mieć problem z rozwiązaniem tego zadania, poproś o pomoc na odpowiednim kanale na Slacku, tj. `s5e06-php-refactoring` (dotyczy [mentee](https://devmentor.pl/mentoring-javascript/)) lub na ogólnodostępnej i bezpłatnej [społeczności na Discordzie](https://devmentor.pl/discord). Pamiętaj, aby treść Twojego wpisu spełniała [odpowiednie kryteria](https://devmentor.pl/jak-prosic-o-pomoc/).*

&nbsp;

# `#04` PHP: Refactoring Techniques

Zastanów sie w jaki sposób do tej pory dodawałeś middleware-y do routera.

Czy Towje rozwiązanie jest w pełni elastyczne? Czy Spełnia założenia [zasady otwarte-zamknięte] tj. OCP(https://pl.wikipedia.org/wiki/Zasada_otwarte-zamkni%C4%99te)?

Głownie chodzi o to, aby móc dodawać funkcjonalność bez potrzeby modyfikowania docelowej klasy. W naszym przypadku chcemy mieć działający router, z możliwością dodawania nowych middleware, bez potrzeby modyfikowania klasy `Router`.

Można to zrobić na zasadzie:

```
$router = new Router();
$router->addMiddleware('*', new LoggerMiddleware()); // każda ścieżka, zapisuj informacje o akcjach
$router->addMiddleware('/admin', new AuthMiddleware()); // ścieżka zaczynająca się od admin, sprawdzaj zalogowanie
```

Dostosuj to rozwiązanie do swojej klasy.


&nbsp;
> :no_entry: *Jeśli nie posiadasz materiałów do tego zadania tj. **Wideo**, znajdziesz je na stronie [laracasts.com](https://laracasts.com/referral/bogolubow)*

> :arrow_left: [*poprzednie zadanie*](./../03) | [*następne zadanie*](./../05) :arrow_right:
