# UI Frame

-- Get Start
```c++
auto frame = ekg::frame();
auto button = ekg::button("Button");

frame->place(button, 10, 10);

button->set_pos(20, 20); // Now the pos of button is scaled.
button->get_master_id(); // frame id.
```

-- Setters
```c++
frame->set_width(200);
frame->set_height(200);

frame->set_min_width(50); // limit of limit is 10;
frame->set_min_height(50);

frame->set_resize_dock(ekg::dock::FULL);
frame->set_resize_offset(1.0f);

frame->set_drag_dock(ekg::dock::TOP_LEFT);
frame->set_drag_offset(1.0f);
```

-- Getters
```c++
frame->get_width();
frame->get_height();

frame->get_min_width();
frame->get_min_height();

frame->get_resize_dock();
frame->get_resize_offset();

frame->get_drag_dock();
frame->get_drag_offset();
```