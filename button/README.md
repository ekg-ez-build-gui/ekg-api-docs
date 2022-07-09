# UI Button

Get start!
The EKG button has many options and methods.

```c++
auto button = ekg::button("hi-auto");
ekg_button* button = ekg::button("hi-no-auto");
```

-- Usage
```c++
if (sdl_event.type == SDL_FINGERDOWN || sdl_event.type == SDL_MOUSEBUTTONDOWN) {

	if (button->get_callback_flag()) {
		std::cout << "Button clicked!" << std::endl;
	}
}
```

-- Setters
```c++
button->set_width(75.0f);
button->set_size(12.0f); // min height + 6.0f;

button->set_pos(10.0f, 10.0f);
button->set_x(10.0f);
button->set_y(10.0f);

button->set_text("hi");
button->set_text_offset(2.0f);
button->set_text_aligment(ekg::dock::CENTER);

button->set_callback_flag(false);
button->set_click_flag(true);
button->set_highlight_flag(false);

button->set_visibility(ekg::visibility::VISIBLE);
button->set_state(true);
```

-- Getters
```c++
button->get_width();
button->get_height();
button->get_size();

button->get_x();
button->get_y();

button->get_text();
button->get_text_offset();
button->get_text_aligment();

button->get_callback_flag();
button->get_click_flag();
button->get_highlight_flag();

button->get_min_width();
button->get_min_height();

button->get_state();
```
