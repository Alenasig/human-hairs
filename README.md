# human-hairs
def calculate_number_of_hairs():
    # Constants and assumptions
    average_hair_density_per_square_inch = 200 # average hair density on scalp
    scalp_surface_area_sq_inches = 100  # assumed scalp surface area in square inches
    average_hair_length_inches = 12  # average hair length in inches

    # Calculate the volume of hair assuming cylindrical shape
    volume_of_one_hair_cubic_inches = average_hair_length_inches * 0.01  # assuming a thin hair diameter
    total_volume_of_hair_cubic_inches = volume_of_one_hair_cubic_inches * average_hair_density_per_square_inch * scalp_surface_area_sq_inches

    # Calculate the number of hairs
    total_number_of_hairs = total_volume_of_hair_cubic_inches / volume_of_one_hair_cubic_inches

    return total_number_of_hairs

estimated_number_of_hairs = calculate_number_of_hairs()
print(f"Estimated number of hairs on a human head: {estimated_number_of_hairs:.2e}")
