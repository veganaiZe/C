gtkmm
=====

_Official C++ interface for [GTK](/Libraries/README.md#gtk)_

* [Programming with gtkmm](https://web.archive.org/web/20100804195713id_/http://library.gnome.org/devel/gtkmm-tutorial/stable) - tutorial
  [[pdf](https://www.mrbrklyn.com/resources/programming-with-gtkmm.pdf)]
  [[tar.bz2](https://download.gnome.org/sources/gtkmm-documentation/2.24/gtkmm-documentation-2.24.1.tar.bz2)]
* [gtkmm Reference Manual](https://sources.debian.org/data/main/g/gtkmm2.4/1:2.24.5-6/docs/reference/html/index.html) - v2.24 (2016)
  [[tar.xz](https://download.gnome.org/sources/gtkmm/2.24/gtkmm-2.24.5.tar.xz)]
* [glibmm Reference Manual](https://sources.debian.org/data/main/g/glibmm2.4/2.50.0-1/docs/reference/html/index.html) - v2.50 (2016)
  [[tar.xz](https://download.gnome.org/sources/glibmm/2.50/glibmm-2.50.1.tar.xz)]

---

```c++
// clang++ file.cpp -Wno-deprecated `pkg-config --cflags --libs gtkmm-2.4`

#include <gtkmm.h>  /* All of gtkmm; ~1 megabyte of headers */

int main(int argc, char * argv[])
{
    /* Initialize gtkmm & parse standard command line options */
    Gtk::Main kit (argc, argv);

    /* Create a window */
    Gtk::Window window;

    /* Display window & enter gtkmm main processing loop until window closed */
    Gtk::Main::run(window);
}
```


* `T* Gtk::manage(T* gtk_object)` makes child widget owned by its parent container so it's deleted automatically.
* `GtkObject* Gtk::Object::gobj()` to access underlying C `GtkObject`. (e.g. `button->gobj()`)
* `Glib::wrap(GObject* object, bool take_copy=false)` create C++ gtkmm wrapper object instance from C `GObject` instance. (`take_copy=true` increments C instance's ref count)
* `Glib::ustring` similar interface as `std::string` but contains utf-8 unicode characters. `<glibmm/ustring.h>`
* Don't use ~~`Glib::StringArrayHandle`~~ or ~~`Glib::ArrayHandle<Glib::ustring>`~~
  - Use `std::vector<Glib::ustring>`, `std::list<Glib::ustring>`, `const char*[]`, etc.
* Don't use ~~`Glib::ListHandle<Gtk::Widget*>`~~ or ~~`Glib::SListHandle<Gtk::Widget*>`~~
  - Use `std::vector<Gtk::Widget*>`, `std::list<Gtk::Widget*>`, etc.
