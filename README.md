# q1uq1utrain.github.io

all_points = []

heart_halo_point = set()
for _ in range(halo_number):
    t = random.uniform(0, 2 * pi)
    x, y = heart_function(t, shrink_ratio=11.5
    x, y = shrink(x, y, halo_radius)
    if (x, y) not in heart_halo_point:
        heart_halo_point.add((x, y))
        x += random.randint(-14, 14)
        y += random.randint(-14, 14)
        size = random.choice((1, 2, 2))
        all_points.append((x, y, size))
