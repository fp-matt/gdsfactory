

Generic PDK
=============================

Parametric Cells for the Generic PDK.

Consider them a foundation from which you can draw inspiration. Feel free to modify their cross-sections and layers to tailor a unique PDK suited for any foundry of your choice.

By doing so, you'll possess a versatile, retargetable PDK, empowering you to design your circuits with speed and flexibility.



C
----------------------------------------------------

.. autofunction:: gdsfactory.components.C

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.C(width=1, size=(10, 20), layer='WG', port_type='electrical')
  c.plot()



L
----------------------------------------------------

.. autofunction:: gdsfactory.components.L

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.L(width=1, size=(10, 20), layer='MTOP', port_type='electrical')
  c.plot()



add_fiber_array_optical_south_electrical_north
----------------------------------------------------

.. autofunction:: gdsfactory.components.add_fiber_array_optical_south_electrical_north

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.add_fiber_array_optical_south_electrical_north(with_loopback=True, pad_spacing=100, fiber_spacing=127, pad_gc_spacing=250, electrical_port_orientation=90)
  c.plot()



add_frame
----------------------------------------------------

.. autofunction:: gdsfactory.components.add_frame

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.add_frame(width=10, spacing=10, layer='WG')
  c.plot()



add_termination
----------------------------------------------------

.. autofunction:: gdsfactory.components.add_termination

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.add_termination(component='straight')
  c.plot()



add_trenches
----------------------------------------------------

.. autofunction:: gdsfactory.components.add_trenches

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.add_trenches(layer_component='WG', layer_trench='DEEP_ETCH', width_trench=2, cross_section='rib_with_trenches', right=0, left=0)
  c.plot()



add_trenches90
----------------------------------------------------

.. autofunction:: gdsfactory.components.add_trenches90

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.add_trenches90(layer_component='WG', layer_trench='DEEP_ETCH', width_trench=2, cross_section='rib_with_trenches', top=0, left=0)
  c.plot()



align_wafer
----------------------------------------------------

.. autofunction:: gdsfactory.components.align_wafer

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.align_wafer(width=10, spacing=10, cross_length=80, layer='WG', square_corner='bottom_left')
  c.plot()



array
----------------------------------------------------

.. autofunction:: gdsfactory.components.array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.array(component='pad', spacing=(150, 150), columns=6, rows=1, add_ports=True, centered=False)
  c.plot()



bbox
----------------------------------------------------

.. autofunction:: gdsfactory.components.bbox

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bbox(top=0, bottom=0, left=0, right=0)
  c.plot()



bend_circular
----------------------------------------------------

.. autofunction:: gdsfactory.components.bend_circular

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bend_circular(angle=90, cross_section='strip', allow_min_radius_violation=False)
  c.plot()



bend_circular_heater
----------------------------------------------------

.. autofunction:: gdsfactory.components.bend_circular_heater

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bend_circular_heater(angle=90, heater_to_wg_distance=1.2, heater_width=0.5, layer_heater='HEATER', cross_section='strip', allow_min_radius_violation=False)
  c.plot()



bend_euler
----------------------------------------------------

.. autofunction:: gdsfactory.components.bend_euler

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bend_euler(angle=90, p=0.5, with_arc_floorplan=True, cross_section='strip', allow_min_radius_violation=False)
  c.plot()



bend_euler_s
----------------------------------------------------

.. autofunction:: gdsfactory.components.bend_euler_s

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bend_euler_s()
  c.plot()



bend_euler_trenches
----------------------------------------------------

.. autofunction:: gdsfactory.components.bend_euler_trenches

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bend_euler_trenches(layer_component='WG', layer_trench='DEEP_ETCH', width_trench=2, cross_section='rib_with_trenches', top=0, left=0)
  c.plot()



bend_s
----------------------------------------------------

.. autofunction:: gdsfactory.components.bend_s

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bend_s(size=(11, 1.8), npoints=99, cross_section='strip', allow_min_radius_violation=False)
  c.plot()



bezier
----------------------------------------------------

.. autofunction:: gdsfactory.components.bezier

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.bezier(control_points=((0, 0), (5, 0), (5, 1.8), (10, 1.8)), npoints=201, with_manhattan_facing_angles=True, cross_section='strip', allow_min_radius_violation=False)
  c.plot()



cavity
----------------------------------------------------

.. autofunction:: gdsfactory.components.cavity

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cavity(coupler='coupler', length=0.1, gap=0.2)
  c.plot()



cdsem_all
----------------------------------------------------

.. autofunction:: gdsfactory.components.cdsem_all

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cdsem_all(widths=(0.4, 0.45, 0.5, 0.6, 0.8, 1), dense_lines_width=0.3, dense_lines_width_difference=0.02, dense_lines_gap=0.3, dense_lines_labels=('DL', 'DM', 'DH'), straight='straight', bend90='bend_circular', cross_section='strip', spacing=5)
  c.plot()



cdsem_bend180
----------------------------------------------------

.. autofunction:: gdsfactory.components.cdsem_bend180

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cdsem_bend180(width=0.5, radius=10, wg_length=420, straight='straight', bend90='bend_circular', cross_section='strip')
  c.plot()



cdsem_coupler
----------------------------------------------------

.. autofunction:: gdsfactory.components.cdsem_coupler

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cdsem_coupler(length=420, gaps=(0.15, 0.2, 0.25), cross_section='strip', spacing=7)
  c.plot()



cdsem_straight
----------------------------------------------------

.. autofunction:: gdsfactory.components.cdsem_straight

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cdsem_straight(widths=(0.4, 0.45, 0.5, 0.6, 0.8, 1), length=420, cross_section='strip', text='text_rectangular_mini', spacing=7)
  c.plot()



cdsem_straight_density
----------------------------------------------------

.. autofunction:: gdsfactory.components.cdsem_straight_density

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cdsem_straight_density(widths=(0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3), gaps=(0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3, 0.3), length=420, label='', cross_section='strip')
  c.plot()



circle
----------------------------------------------------

.. autofunction:: gdsfactory.components.circle

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.circle(radius=10, angle_resolution=2.5, layer='WG')
  c.plot()



coh_rx_single_pol
----------------------------------------------------

.. autofunction:: gdsfactory.components.coh_rx_single_pol

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coh_rx_single_pol(bend='bend_euler', cross_section='strip', det_spacing=(60, 50), in_wg_length=20, cross_section_metal_top='metal3', cross_section_metal='metal2')
  c.plot()



coh_tx_dual_pol
----------------------------------------------------

.. autofunction:: gdsfactory.components.coh_tx_dual_pol

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coh_tx_dual_pol(splitter='mmi1x2', spol_coh_tx='coh_tx_single_pol', yspacing=10, xspacing=40, cross_section='strip')
  c.plot()



coh_tx_single_pol
----------------------------------------------------

.. autofunction:: gdsfactory.components.coh_tx_single_pol

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coh_tx_single_pol(balanced_phase_shifters=False, mzm_y_spacing=50, phase_shifter='straight_pin', phase_shifter_length=100, mzm_ps_spacing=40, splitter='mmi1x2', mzm='mzi_pin', mzm_length=200, xspacing=40, pad_array='pad_array', cross_section='strip')
  c.plot()



compass
----------------------------------------------------

.. autofunction:: gdsfactory.components.compass

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.compass(size=(4, 2), layer='WG', port_type='electrical', port_inclusion=0, port_orientations=(180, 90, 0, -90))
  c.plot()



component_sequence
----------------------------------------------------

.. autofunction:: gdsfactory.components.component_sequence



copy_layers
----------------------------------------------------

.. autofunction:: gdsfactory.components.copy_layers

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.copy_layers(layers=((1, 0), (2, 0)))
  c.plot()



coupler
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler(gap=0.236, length=20, dy=4, dx=10, cross_section='strip')
  c.plot()



coupler90
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler90

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler90(gap=0.2, radius=10, cross_section='strip')
  c.plot()



coupler90bend
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler90bend

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler90bend(radius=10, gap=0.2, cross_section_inner='strip', cross_section_outer='strip')
  c.plot()



coupler90circular
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler90circular

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler90circular(gap=0.2, radius=10, cross_section='strip')
  c.plot()



coupler_adiabatic
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_adiabatic

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_adiabatic(length1=20, length2=50, length3=30, wg_sep=1, input_wg_sep=3, output_wg_sep=3, dw=0.1, cross_section='strip')
  c.plot()



coupler_asymmetric
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_asymmetric

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_asymmetric(gap=0.234, dy=2.5, dx=10, cross_section='strip')
  c.plot()



coupler_bend
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_bend

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_bend(radius=10, coupler_gap=0.2, coupling_angle_coverage=120, cross_section_inner='strip', cross_section_outer='strip')
  c.plot()



coupler_bent
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_bent

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_bent(gap=0.2, radius=26, length=8.6, width1=0.4, width2=0.4, length_straight=10, cross_section='strip')
  c.plot()



coupler_broadband
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_broadband

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_broadband(w_sc=0.5, gap_sc=0.2, w_top=0.6, gap_pc=0.3, legnth_taper=1, length_coupler_straight=12.4, lenght_coupler_big_gap=4.7, cross_section='strip', radius=10)
  c.plot()



coupler_full
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_full

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_full(coupling_length=40, dx=10, dy=4.8, gap=0.5, dw=0.1, cross_section='strip')
  c.plot()



coupler_ring
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_ring

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_ring(gap=0.2, radius=5, length_x=4, cross_section='strip', length_extension=3)
  c.plot()



coupler_straight
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_straight

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_straight(length=10, gap=0.27, cross_section='strip')
  c.plot()



coupler_straight_asymmetric
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_straight_asymmetric

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_straight_asymmetric(length=10, gap=0.27, width_top=0.5, width_bot=1, cross_section='strip')
  c.plot()



coupler_symmetric
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_symmetric

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_symmetric(gap=0.234, dy=4, dx=10, cross_section='strip')
  c.plot()



coupler_trenches
----------------------------------------------------

.. autofunction:: gdsfactory.components.coupler_trenches

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.coupler_trenches(layer_component='WG', layer_trench='DEEP_ETCH', width_trench=2, cross_section='rib_with_trenches', right=0, left=0)
  c.plot()



cross
----------------------------------------------------

.. autofunction:: gdsfactory.components.cross

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cross(length=10, width=3, layer='WG')
  c.plot()



crossing
----------------------------------------------------

.. autofunction:: gdsfactory.components.crossing

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.crossing(cross_section='strip')
  c.plot()



crossing45
----------------------------------------------------

.. autofunction:: gdsfactory.components.crossing45

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.crossing45(port_spacing=40, alpha=0.08, npoints=101, cross_section='strip', cross_section_bends='strip')
  c.plot()



crossing_arm
----------------------------------------------------

.. autofunction:: gdsfactory.components.crossing_arm

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.crossing_arm(r1=3, r2=1.1, w=1.2, L=3.4, layer_slab='SLAB150', cross_section='strip')
  c.plot()



crossing_etched
----------------------------------------------------

.. autofunction:: gdsfactory.components.crossing_etched

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.crossing_etched(width=0.5, r1=3, r2=1.1, w=1.2, L=3.4, layer_wg='WG', layer_slab='SLAB150')
  c.plot()



crossing_from_taper
----------------------------------------------------

.. autofunction:: gdsfactory.components.crossing_from_taper

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.crossing_from_taper()
  c.plot()



cutback_2x2
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_2x2

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_2x2(cols=4, rows=5, port1='o1', port2='o2', port3='o3', port4='o4', mirror=False, cross_section='strip')
  c.plot()



cutback_bend
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_bend

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_bend(straight_length=5, rows=6, cols=5)
  c.plot()



cutback_bend180
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_bend180

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_bend180(straight_length=5, rows=6, cols=6, spacing=3)
  c.plot()



cutback_bend180circular
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_bend180circular

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_bend180circular(straight_length=5, rows=6, cols=6, spacing=3)
  c.plot()



cutback_bend90
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_bend90

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_bend90(straight_length=5, rows=6, cols=6, spacing=5)
  c.plot()



cutback_bend90circular
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_bend90circular

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_bend90circular(straight_length=5, rows=6, cols=6, spacing=5)
  c.plot()



cutback_component
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_component

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_component(cols=4, rows=5, port1='o1', port2='o2', mirror=False, mirror1=False, mirror2=False, cross_section='strip')
  c.plot()



cutback_component_mirror
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_component_mirror

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_component_mirror(cols=4, rows=5, port1='o1', port2='o2', mirror=True, mirror1=False, mirror2=False, cross_section='strip')
  c.plot()



cutback_splitter
----------------------------------------------------

.. autofunction:: gdsfactory.components.cutback_splitter

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.cutback_splitter(cols=4, rows=5, port1='o1', port2='o2', port3='o3', mirror=False, cross_section='strip')
  c.plot()



dbr
----------------------------------------------------

.. autofunction:: gdsfactory.components.dbr

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.dbr(w1=0.45, w2=0.55, l1=0.159, l2=0.159, n=10, cross_section='strip', straight_length=0.01)
  c.plot()



dbr_tapered
----------------------------------------------------

.. autofunction:: gdsfactory.components.dbr_tapered

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.dbr_tapered(length=10, period=0.85, dc=0.5, w1=0.4, w2=1, taper_length=20, fins=False, fin_size=(0.2, 0.05), cross_section='strip')
  c.plot()



delay_snake
----------------------------------------------------

.. autofunction:: gdsfactory.components.delay_snake

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.delay_snake(length=1600, length0=0, length2=0, n=2, cross_section='strip')
  c.plot()



delay_snake2
----------------------------------------------------

.. autofunction:: gdsfactory.components.delay_snake2

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.delay_snake2(length=1600, length0=0, length2=0, n=2, bend180='bend_euler180', cross_section='strip')
  c.plot()



delay_snake_sbend
----------------------------------------------------

.. autofunction:: gdsfactory.components.delay_snake_sbend

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.delay_snake_sbend(length=100, length1=0, length4=0, radius=5, waveguide_spacing=5, bend='bend_euler', sbend='bend_s', sbend_xsize=100, cross_section='strip')
  c.plot()



dicing_lane
----------------------------------------------------

.. autofunction:: gdsfactory.components.dicing_lane

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.dicing_lane(size=(50, 300), layer_dicing='DICING')
  c.plot()



die
----------------------------------------------------

.. autofunction:: gdsfactory.components.die

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.die(size=(10000, 10000), street_width=100, street_length=1000, die_name='chip99', text_size=100, text_location='SW', layer='FLOORPLAN', bbox_layer='FLOORPLAN', draw_corners=False)
  c.plot()



die_bbox
----------------------------------------------------

.. autofunction:: gdsfactory.components.die_bbox

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.die_bbox(street_width=100, text_size=100, text_anchor='sw', layer='MTOP', padding=10)
  c.plot()



die_with_pads
----------------------------------------------------

.. autofunction:: gdsfactory.components.die_with_pads

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.die_with_pads(size=(11470, 4900), ngratings=14, npads=31, grating_pitch=250, pad_pitch=300, grating_coupler='grating_coupler_te', cross_section='strip', pad='pad', layer_floorplan=32, edge_to_pad_distance=150, edge_to_grating_distance=150)
  c.plot()



disk
----------------------------------------------------

.. autofunction:: gdsfactory.components.disk

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.disk(radius=10, gap=0.2, wrap_angle_deg=180, parity=1, cross_section='strip')
  c.plot()



disk_heater
----------------------------------------------------

.. autofunction:: gdsfactory.components.disk_heater

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.disk_heater(radius=10, gap=0.2, wrap_angle_deg=180, parity=1, cross_section='strip', heater_layer='HEATER', via_stack='via_stack_heater_mtop', heater_width=5, heater_extent=2, via_width=10, port_orientation=90)
  c.plot()



edge_coupler_array
----------------------------------------------------

.. autofunction:: gdsfactory.components.edge_coupler_array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.edge_coupler_array(n=5, pitch=127, x_reflection=False, text_offset=(10, 20), text_rotation=0)
  c.plot()



edge_coupler_array_with_loopback
----------------------------------------------------

.. autofunction:: gdsfactory.components.edge_coupler_array_with_loopback

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.edge_coupler_array_with_loopback(cross_section='strip', radius=30, n=8, pitch=127, extension_length=1, x_reflection=False, text_offset=(0, 10), text_rotation=0)
  c.plot()



edge_coupler_silicon
----------------------------------------------------

.. autofunction:: gdsfactory.components.edge_coupler_silicon

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.edge_coupler_silicon(length=100, width1=0.5, width2=0.2, with_two_ports=True, cross_section='strip', port_names=('o1', 'o2'), port_types=('optical', 'optical'), with_bbox=True)
  c.plot()



ellipse
----------------------------------------------------

.. autofunction:: gdsfactory.components.ellipse

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ellipse(radii=(10, 5), angle_resolution=2.5, layer='WG')
  c.plot()



extend_ports
----------------------------------------------------

.. autofunction:: gdsfactory.components.extend_ports

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.extend_ports(length=5, port_type='optical', centered=False)
  c.plot()



extend_ports_list
----------------------------------------------------

.. autofunction:: gdsfactory.components.extend_ports_list



fiber
----------------------------------------------------

.. autofunction:: gdsfactory.components.fiber

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.fiber(core_diameter=10, cladding_diameter=125, layer_core='WG', layer_cladding='WGCLAD')
  c.plot()



fiber_array
----------------------------------------------------

.. autofunction:: gdsfactory.components.fiber_array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.fiber_array(n=8, pitch=127, core_diameter=10, cladding_diameter=125, layer_core='WG', layer_cladding='WGCLAD')
  c.plot()



fiducial_squares
----------------------------------------------------

.. autofunction:: gdsfactory.components.fiducial_squares

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.fiducial_squares(layers=((1, 0),), size=(5, 5), offset=0.14)
  c.plot()



ge_detector_straight_si_contacts
----------------------------------------------------

.. autofunction:: gdsfactory.components.ge_detector_straight_si_contacts

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ge_detector_straight_si_contacts(length=80, via_stack_width=10, via_stack_spacing=5, via_stack_offset=0)
  c.plot()



grating_coupler_array
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_array(pitch=127, n=6, port_name='o1', rotation=-90, with_loopback=False, cross_section='strip', straight_to_grating_spacing=10, centered=True)
  c.plot()



grating_coupler_dual_pol
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_dual_pol

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_dual_pol(period_x=0.58, period_y=0.58, x_span=11, y_span=11, length_taper=150, width_taper=10, polarization='dual', wavelength=1.55, base_layer='WG', cross_section='strip')
  c.plot()



grating_coupler_elliptical
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_elliptical

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_elliptical(polarization='te', taper_length=16.6, taper_angle=40, wavelength=1.554, fiber_angle=15, grating_line_width=0.343, neff=2.638, nclad=1.443, n_periods=30, big_last_tooth=False, layer_slab='SLAB150', slab_xmin=-1, slab_offset=2, spiked=True, cross_section='strip')
  c.plot()



grating_coupler_elliptical_arbitrary
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_elliptical_arbitrary

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_elliptical_arbitrary(gaps=(0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1), widths=(0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5), taper_length=16.6, taper_angle=60, wavelength=1.554, fiber_angle=15, nclad=1.443, layer_slab='SLAB150', taper_to_slab_offset=-3, polarization='te', spiked=True, bias_gap=0, cross_section='strip')
  c.plot()



grating_coupler_elliptical_lumerical
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_elliptical_lumerical

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_elliptical_lumerical(parameters=(-2.43, 0.1, 0.48, 0.1, 0.607, 0.1, 0.45, 0.1, 0.427, 0.1, 0.476, 0.1, 0.503, 0.1, 0.51, 0.1, 0.494, 0.108, 0.474, 0.15, 0.433, 0.184, 0.387, 0.236, 0.36, 0.243, 0.358, 0.261, 0.353, 0.247, 0.372, 0.229, 0.378, 0.225, 0.377, 0.22, 0.38, 0.219, 0.38, 0.217, 0.383, 0.218, 0.364, 0.237, 0.368, 0.249, 0.344, 0.273, 0.331, 0.274), layer='WG', layer_slab='SLAB150', taper_angle=55, taper_length=12.6, fiber_angle=5, bias_gap=0)
  c.plot()



grating_coupler_elliptical_trenches
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_elliptical_trenches

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_elliptical_trenches(polarization='te', taper_length=16.6, taper_angle=30, trenches_extra_angle=9, wavelength=1.53, fiber_angle=15, grating_line_width=0.343, neff=2.638, ncladding=1.443, layer_trench='SHALLOW_ETCH', p_start=26, n_periods=30, end_straight_length=0.2, cross_section='strip')
  c.plot()



grating_coupler_elliptical_uniform
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_elliptical_uniform

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_elliptical_uniform(n_periods=20, period=0.75, fill_factor=0.5)
  c.plot()



grating_coupler_loss_fiber_array
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_loss_fiber_array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_loss_fiber_array(pitch=127, port_name='o1', cross_section='strip', rotation=-90)
  c.plot()



grating_coupler_loss_fiber_array4
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_loss_fiber_array4

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_loss_fiber_array4(pitch=127)
  c.plot()



grating_coupler_rectangular
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_rectangular

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_rectangular(n_periods=20, period=0.75, fill_factor=0.5, width_grating=11, length_taper=150, polarization='te', wavelength=1.55, layer_slab='SLAB150', fiber_angle=15, slab_xmin=-1, slab_offset=1, cross_section='strip')
  c.plot()



grating_coupler_rectangular_arbitrary
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_rectangular_arbitrary

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_rectangular_arbitrary(gaps=(0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2, 0.2), widths=(0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5), width_grating=11, length_taper=150, polarization='te', wavelength=1.55, slab_xmin=-1, slab_offset=1, fiber_angle=15, cross_section='strip')
  c.plot()



grating_coupler_tree
----------------------------------------------------

.. autofunction:: gdsfactory.components.grating_coupler_tree

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.grating_coupler_tree(n=4, straight_spacing=4, with_loopback=False, bend='bend_euler', fanout_length=0)
  c.plot()



greek_cross
----------------------------------------------------

.. autofunction:: gdsfactory.components.greek_cross

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.greek_cross(length=30, layers=('WG', 'N'), widths=(2, 3), via_stack='via_stack_npp_m1')
  c.plot()



greek_cross_with_pads
----------------------------------------------------

.. autofunction:: gdsfactory.components.greek_cross_with_pads

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.greek_cross_with_pads(pad='pad', pad_spacing=150, greek_cross_component='greek_cross', pad_via='via_stack_m1_mtop')
  c.plot()



hexagon
----------------------------------------------------

.. autofunction:: gdsfactory.components.hexagon

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.hexagon(sides=6, side_length=10, layer='WG', port_type='placement')
  c.plot()



hline
----------------------------------------------------

.. autofunction:: gdsfactory.components.hline

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.hline(length=10, width=0.5, layer='WG', port_type='optical')
  c.plot()



interdigital_capacitor
----------------------------------------------------

.. autofunction:: gdsfactory.components.interdigital_capacitor

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.interdigital_capacitor(fingers=4, finger_length=20, finger_gap=2, thickness=5, layer='WG')
  c.plot()



litho_calipers
----------------------------------------------------

.. autofunction:: gdsfactory.components.litho_calipers

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.litho_calipers(notch_size=(2, 5), notch_spacing=2, num_notches=11, offset_per_notch=0.1, row_spacing=0, layer1='WG', layer2='SLAB150')
  c.plot()



litho_ruler
----------------------------------------------------

.. autofunction:: gdsfactory.components.litho_ruler

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.litho_ruler(height=2, width=0.5, spacing=2, scale=(3, 1, 1, 1, 1, 2, 1, 1, 1, 1), num_marks=21, layer='WG')
  c.plot()



litho_steps
----------------------------------------------------

.. autofunction:: gdsfactory.components.litho_steps

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.litho_steps(line_widths=(1, 2, 4, 8, 16), line_spacing=10, height=100, layer='WG')
  c.plot()



loop_mirror
----------------------------------------------------

.. autofunction:: gdsfactory.components.loop_mirror

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.loop_mirror(component='mmi1x2', bend90='bend_euler')
  c.plot()



loss_deembedding_ch12_34
----------------------------------------------------

.. autofunction:: gdsfactory.components.loss_deembedding_ch12_34

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.loss_deembedding_ch12_34(pitch=127, port_name='o1', cross_section='strip', rotation=-90)
  c.plot()



loss_deembedding_ch13_24
----------------------------------------------------

.. autofunction:: gdsfactory.components.loss_deembedding_ch13_24

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.loss_deembedding_ch13_24(pitch=127, cross_section='strip', port_name='o1', rotation=-90)
  c.plot()



loss_deembedding_ch14_23
----------------------------------------------------

.. autofunction:: gdsfactory.components.loss_deembedding_ch14_23

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.loss_deembedding_ch14_23(pitch=127, cross_section='strip', port_name='o1', rotation=-90)
  c.plot()



mmi
----------------------------------------------------

.. autofunction:: gdsfactory.components.mmi

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mmi(inputs=1, outputs=4, width_taper=1, length_taper=10, length_mmi=5.5, width_mmi=5, gap_input_tapers=0.25, gap_output_tapers=0.25, cross_section='strip')
  c.plot()



mmi1x2
----------------------------------------------------

.. autofunction:: gdsfactory.components.mmi1x2

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mmi1x2(width_taper=1, length_taper=10, length_mmi=5.5, width_mmi=2.5, gap_mmi=0.25, cross_section='strip')
  c.plot()



mmi1x2_with_sbend
----------------------------------------------------

.. autofunction:: gdsfactory.components.mmi1x2_with_sbend

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mmi1x2_with_sbend(with_sbend=True, cross_section='strip')
  c.plot()



mmi2x2
----------------------------------------------------

.. autofunction:: gdsfactory.components.mmi2x2

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mmi2x2(width_taper=1, length_taper=10, length_mmi=5.5, width_mmi=2.5, gap_mmi=0.25, cross_section='strip')
  c.plot()



mmi2x2_with_sbend
----------------------------------------------------

.. autofunction:: gdsfactory.components.mmi2x2_with_sbend

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mmi2x2_with_sbend(with_sbend=True, cross_section='strip')
  c.plot()



mmi_90degree_hybrid
----------------------------------------------------

.. autofunction:: gdsfactory.components.mmi_90degree_hybrid

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mmi_90degree_hybrid(width=0.5, width_taper=1.7, length_taper=40, length_mmi=175, width_mmi=10, gap_mmi=0.8, cross_section='strip')
  c.plot()



mode_converter
----------------------------------------------------

.. autofunction:: gdsfactory.components.mode_converter

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mode_converter(gap=0.3, length=10, mm_width=1.2, mc_mm_width=1, sm_width=0.5, taper_length=25, cross_section='strip')
  c.plot()



mzi
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi(delta_length=10, length_y=2, length_x=0.1, splitter='mmi1x2', with_splitter=True, port_e1_splitter='o2', port_e0_splitter='o3', port_e1_combiner='o2', port_e0_combiner='o3', nbends=2, cross_section='strip', mirror_bot=False, add_optical_ports_arms=False, min_length=0.01, auto_rename_ports=True)
  c.plot()



mzi1x2_2x2
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi1x2_2x2

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi1x2_2x2(delta_length=10, length_y=2, length_x=0.1, splitter='mmi1x2', with_splitter=True, port_e1_splitter='o2', port_e0_splitter='o3', port_e1_combiner='o3', port_e0_combiner='o4', nbends=2, cross_section='strip', mirror_bot=False, add_optical_ports_arms=False, min_length=0.01, auto_rename_ports=True)
  c.plot()



mzi2x2_2x2_phase_shifter
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi2x2_2x2_phase_shifter

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi2x2_2x2_phase_shifter(delta_length=10, length_y=2, length_x=200, straight_x_top='straight_heater_metal', with_splitter=True, port_e1_splitter='o3', port_e0_splitter='o4', port_e1_combiner='o3', port_e0_combiner='o4', nbends=2, cross_section='strip', mirror_bot=False, add_optical_ports_arms=False, min_length=0.01, auto_rename_ports=True)
  c.plot()



mzi_arm
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi_arm

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi_arm(length_y_left=0.8, length_y_right=0.8, length_x=0.1)
  c.plot()



mzi_lattice
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi_lattice

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi_lattice(coupler_lengths=(10, 20), coupler_gaps=(0.2, 0.3), delta_lengths=(10,), mzi='mzi_coupler', splitter='coupler')
  c.plot()



mzi_lattice_mmi
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi_lattice_mmi

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi_lattice_mmi(coupler_widths=(None, None), coupler_widths_tapers=(1, 1), coupler_lengths_tapers=(10, 10), coupler_lengths_mmis=(5.5, 5.5), coupler_widths_mmis=(2.5, 2.5), coupler_gaps_mmis=(0.25, 0.25), taper_functions_mmis=('taper', 'taper'), straight_functions_mmis=('straight', 'straight'), cross_sections_mmis=('strip', 'strip'), delta_lengths=(10,), mzi='mzi2x2_2x2', splitter='mmi2x2')
  c.plot()



mzi_pads_center
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi_pads_center

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi_pads_center(length_x=500, length_y=40, mzi_sig_top='top_r_e2', mzi_gnd_top='top_l_e2', mzi_sig_bot='bot_l_e2', mzi_gnd_bot='bot_r_e2', pad_sig_bot='e1_1_1', pad_sig_top='e3_1_3', pad_gnd_bot='e4_1_2', pad_gnd_top='e2_1_2', delta_length=40, cross_section='strip', cross_section_metal='metal_routing', pad_spacing='pad_spacing')
  c.plot()



mzi_phase_shifter
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi_phase_shifter

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi_phase_shifter(delta_length=10, length_y=2, length_x=200, straight_x_top='straight_heater_metal', splitter='mmi1x2', with_splitter=True, port_e1_splitter='o2', port_e0_splitter='o3', port_e1_combiner='o2', port_e0_combiner='o3', nbends=2, cross_section='strip', mirror_bot=False, add_optical_ports_arms=False, min_length=0.01, auto_rename_ports=True)
  c.plot()



mzi_phase_shifter_top_heater_metal
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi_phase_shifter_top_heater_metal

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi_phase_shifter_top_heater_metal(delta_length=10, length_y=2, length_x=200, splitter='mmi1x2', with_splitter=True, port_e1_splitter='o2', port_e0_splitter='o3', port_e1_combiner='o2', port_e0_combiner='o3', nbends=2, cross_section='strip', mirror_bot=False, add_optical_ports_arms=False, min_length=0.01, auto_rename_ports=True)
  c.plot()



mzi_pin
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzi_pin

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzi_pin(delta_length=0, length_y=2, length_x=100, straight_x_top='straight_pin', splitter='mmi1x2', with_splitter=True, port_e1_splitter='o2', port_e0_splitter='o3', port_e1_combiner='o2', port_e0_combiner='o3', nbends=2, cross_section='strip', cross_section_x_top='pin', mirror_bot=False, add_optical_ports_arms=False, min_length=0.01, auto_rename_ports=True)
  c.plot()



mzit
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzit

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzit(w0=0.5, w1=0.45, w2=0.55, dy=2, delta_length=10, length=1, coupler_length1=5, coupler_length2=10, coupler_gap1=0.2, coupler_gap2=0.3, taper_length=5, cross_section='strip')
  c.plot()



mzit_lattice
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzit_lattice

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzit_lattice(coupler_lengths=(10, 20), coupler_gaps=(0.2, 0.3), delta_lengths=(10,))
  c.plot()



mzm
----------------------------------------------------

.. autofunction:: gdsfactory.components.mzm

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.mzm(delta_length=10, length_y=2, length_x=200, straight_x_top='straight_pin', straight_x_bot='straight_pin', splitter='mmi1x2', with_splitter=True, port_e1_splitter='o2', port_e0_splitter='o3', port_e1_combiner='o2', port_e0_combiner='o3', nbends=2, cross_section='strip', mirror_bot=False, add_optical_ports_arms=False, min_length=0.01, auto_rename_ports=True)
  c.plot()



nxn
----------------------------------------------------

.. autofunction:: gdsfactory.components.nxn

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.nxn(west=1, east=4, north=0, south=0, xsize=8, ysize=8, wg_width=0.5, layer='WG', wg_margin=1)
  c.plot()



octagon
----------------------------------------------------

.. autofunction:: gdsfactory.components.octagon

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.octagon(sides=8, side_length=10, layer='WG', port_type='placement')
  c.plot()



optimal_90deg
----------------------------------------------------

.. autofunction:: gdsfactory.components.optimal_90deg

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.optimal_90deg(width=100, num_pts=15, length_adjust=1, layer=(1, 0))
  c.plot()



optimal_hairpin
----------------------------------------------------

.. autofunction:: gdsfactory.components.optimal_hairpin

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.optimal_hairpin(width=0.2, pitch=0.6, length=10, turn_ratio=4, num_pts=50, layer=(1, 0))
  c.plot()



optimal_step
----------------------------------------------------

.. autofunction:: gdsfactory.components.optimal_step

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.optimal_step(start_width=10, end_width=22, num_pts=50, width_tol=0.001, anticrowding_factor=1.2, symmetric=False, layer=(1, 0))
  c.plot()



pack_doe
----------------------------------------------------

.. autofunction:: gdsfactory.components.pack_doe

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pack_doe(doe='mmi1x2', do_permutations=False)
  c.plot()



pack_doe_grid
----------------------------------------------------

.. autofunction:: gdsfactory.components.pack_doe_grid

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pack_doe_grid(doe='mmi1x2', do_permutations=False, with_text=False)
  c.plot()



pad
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad(size=(100, 100), layer='MTOP', port_inclusion=0, port_orientation=0)
  c.plot()



pad_array
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_array(pad='pad', spacing=(150, 150), columns=6, rows=1, port_orientation=0, size=(100, 100), layer='MTOP')
  c.plot()



pad_array0
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_array0

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_array0(pad='pad', spacing=(150, 150), columns=1, rows=3, port_orientation=0, size=(100, 100), layer='MTOP')
  c.plot()



pad_array180
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_array180

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_array180(pad='pad', spacing=(150, 150), columns=1, rows=3, port_orientation=180, size=(100, 100), layer='MTOP')
  c.plot()



pad_array270
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_array270

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_array270(pad='pad', spacing=(150, 150), columns=6, rows=1, port_orientation=270, size=(100, 100), layer='MTOP')
  c.plot()



pad_array90
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_array90

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_array90(pad='pad', spacing=(150, 150), columns=6, rows=1, port_orientation=90, size=(100, 100), layer='MTOP')
  c.plot()



pad_gsg_open
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_gsg_open

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_gsg_open(size=(22, 7), layer_metal='MTOP', metal_spacing=5, short=False, pad='pad', pad_spacing=150, route_xsize=50)
  c.plot()



pad_gsg_short
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_gsg_short

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_gsg_short(size=(22, 7), layer_metal='MTOP', metal_spacing=5, short=True, pad='pad', pad_spacing=150, route_xsize=50)
  c.plot()



pad_rectangular
----------------------------------------------------

.. autofunction:: gdsfactory.components.pad_rectangular

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pad_rectangular(size='pad_size', layer='MTOP', port_inclusion=0, port_orientation=0)
  c.plot()



pads_shorted
----------------------------------------------------

.. autofunction:: gdsfactory.components.pads_shorted

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pads_shorted(columns=8, pad_spacing=150, layer_metal='MTOP', metal_width=10)
  c.plot()



pixel
----------------------------------------------------

.. autofunction:: gdsfactory.components.pixel

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.pixel(size=1, layer='WG')
  c.plot()



polarization_splitter_rotator
----------------------------------------------------

.. autofunction:: gdsfactory.components.polarization_splitter_rotator

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.polarization_splitter_rotator(width_taper_in=(0.54, 0.69, 0.83), length_taper_in=(4, 44), width_coupler=(0.9, 0.404), length_coupler=7, gap=0.15, width_out=0.54, length_out=14.33, dy=5, cross_section='strip')
  c.plot()



qrcode
----------------------------------------------------

.. autofunction:: gdsfactory.components.qrcode

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.qrcode(data='mask01', psize=1, layer='WG')
  c.plot()



ramp
----------------------------------------------------

.. autofunction:: gdsfactory.components.ramp

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ramp(length=10, width1=5, width2=8, layer='WG')
  c.plot()



rectangle
----------------------------------------------------

.. autofunction:: gdsfactory.components.rectangle

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.rectangle(size=(4, 2), layer='WG', centered=False, port_type='electrical', port_orientations=(180, 90, 0, -90))
  c.plot()



rectangle_with_slits
----------------------------------------------------

.. autofunction:: gdsfactory.components.rectangle_with_slits

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.rectangle_with_slits(size=(100, 200), layer='WG', layer_slit='SLAB150', centered=False, slit_size=(1, 1), slit_spacing=(20, 20), slit_enclosure=10)
  c.plot()



rectangles
----------------------------------------------------

.. autofunction:: gdsfactory.components.rectangles

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.rectangles(size=(4, 2), offsets=(0, 1), layers=('WG', 'SLAB150'), centered=True)
  c.plot()



regular_polygon
----------------------------------------------------

.. autofunction:: gdsfactory.components.regular_polygon

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.regular_polygon(sides=6, side_length=10, layer='WG', port_type='placement')
  c.plot()



resistance_meander
----------------------------------------------------

.. autofunction:: gdsfactory.components.resistance_meander

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.resistance_meander(pad_size=(50, 50), num_squares=1000, width=1, res_layer='MTOP', pad_layer='MTOP')
  c.plot()



resistance_sheet
----------------------------------------------------

.. autofunction:: gdsfactory.components.resistance_sheet

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.resistance_sheet(width=10, layers=('HEATER',), layer_offsets=(0, 0.2), pad='via_stack_heater_mtop', pad_size=(50, 50), pad_pitch=100, pad_port_name='e4')
  c.plot()



ring
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring(radius=10, width=0.5, angle_resolution=2.5, layer='WG', angle=360)
  c.plot()



ring_crow
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_crow

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_crow(gaps=(0.2, 0.2, 0.2, 0.2), radius=(10, 10, 10), ring_cross_sections=('strip', 'strip', 'strip'), length_x=0, lengths_y=(0, 0, 0), cross_section='strip')
  c.plot()



ring_crow_couplers
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_crow_couplers

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_crow_couplers(radius=(10, 10, 10), bends=({'function': 'bend_circular', 'module': 'gdsfactory.components.bend_circular'}, {'function': 'bend_circular', 'module': 'gdsfactory.components.bend_circular'}, {'function': 'bend_circular', 'module': 'gdsfactory.components.bend_circular'}), ring_cross_sections=('strip', 'strip', 'strip'), couplers=({'function': 'coupler', 'module': 'gdsfactory.components.coupler'}, {'function': 'coupler', 'module': 'gdsfactory.components.coupler'}, {'function': 'coupler', 'module': 'gdsfactory.components.coupler'}, {'function': 'coupler', 'module': 'gdsfactory.components.coupler'}))
  c.plot()



ring_double
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_double

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_double(gap=0.2, radius=10, length_x=0.01, length_y=0.01, cross_section='strip')
  c.plot()



ring_double_heater
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_double_heater

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_double_heater(gap=0.2, radius=10, length_x=1, length_y=0.01, cross_section_heater='heater_metal', cross_section_waveguide_heater='strip_heater_metal', cross_section='strip', via_stack_offset=(1, 0), with_drop=True)
  c.plot()



ring_double_pn
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_double_pn

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_double_pn(add_gap=0.3, drop_gap=0.3, radius=5, doping_angle=85, doped_heater=True, doped_heater_angle_buffer=10, doped_heater_layer='NPP', doped_heater_width=0.5, doped_heater_waveguide_offset=2.175, with_drop=True)
  c.plot()



ring_double_trenches
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_double_trenches

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_double_trenches(layer_component='WG', layer_trench='DEEP_ETCH', width_trench=2, cross_section='rib_with_trenches', right=0, left=0)
  c.plot()



ring_single
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_single

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_single(gap=0.2, radius=10, length_x=4, length_y=0.6, cross_section='strip')
  c.plot()



ring_single_array
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_single_array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_single_array(spacing=5, cross_section='strip')
  c.plot()



ring_single_bend_coupler
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_single_bend_coupler

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_single_bend_coupler(radius=5, gap=0.2, coupling_angle_coverage=180, length_x=0.6, length_y=0.6, cross_section_inner='strip', cross_section_outer='strip')
  c.plot()



ring_single_dut
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_single_dut

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_single_dut(gap=0.2, length_x=4, length_y=0, radius=5, with_component=True, port_name='o1')
  c.plot()



ring_single_heater
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_single_heater

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_single_heater(gap=0.2, radius=10, length_x=1, length_y=0.01, cross_section_heater='heater_metal', cross_section_waveguide_heater='strip_heater_metal', cross_section='strip', via_stack_offset=(1, 0), with_drop=False)
  c.plot()



ring_single_pn
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_single_pn

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_single_pn(gap=0.3, radius=5, doping_angle=250, doped_heater=True, doped_heater_angle_buffer=10, doped_heater_layer='NPP', doped_heater_width=0.5, doped_heater_waveguide_offset=2.175)
  c.plot()



ring_single_trenches
----------------------------------------------------

.. autofunction:: gdsfactory.components.ring_single_trenches

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.ring_single_trenches(layer_component='WG', layer_trench='DEEP_ETCH', width_trench=2, cross_section='rib_with_trenches', right=0, left=0)
  c.plot()



seal_ring
----------------------------------------------------

.. autofunction:: gdsfactory.components.seal_ring

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.seal_ring(width=10, padding=10, with_north=True, with_south=True, with_east=True, with_west=True)
  c.plot()



snspd
----------------------------------------------------

.. autofunction:: gdsfactory.components.snspd

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.snspd(wire_width=0.2, wire_pitch=0.6, size=(10, 8), turn_ratio=4, terminals_same_side=False, layer=(1, 0))
  c.plot()



spiral
----------------------------------------------------

.. autofunction:: gdsfactory.components.spiral

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.spiral(length=100, bend='bend_euler', straight='straight', cross_section='strip', spacing=3, n_loops=6)
  c.plot()



spiral_double
----------------------------------------------------

.. autofunction:: gdsfactory.components.spiral_double

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.spiral_double(min_bend_radius=10, separation=2, number_of_loops=3, npoints=1000, cross_section='strip')
  c.plot()



spiral_racetrack
----------------------------------------------------

.. autofunction:: gdsfactory.components.spiral_racetrack

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.spiral_racetrack(min_radius=5, straight_length=20, spacings=(2, 2, 3, 3, 2, 2), cross_section='strip', n_bend_points=99, with_inner_ports=False, extra_90_deg_bend=False)
  c.plot()



spiral_racetrack_fixed_length
----------------------------------------------------

.. autofunction:: gdsfactory.components.spiral_racetrack_fixed_length

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.spiral_racetrack_fixed_length(length=1000, in_out_port_spacing=150, n_straight_sections=8, min_radius=5, min_spacing=5, cross_section='strip', n_bend_points=99, with_inner_ports=False)
  c.plot()



spiral_racetrack_heater_doped
----------------------------------------------------

.. autofunction:: gdsfactory.components.spiral_racetrack_heater_doped

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.spiral_racetrack_heater_doped(straight_length=30, spacing=2, num=8, waveguide_cross_section='strip', heater_cross_section='npp')
  c.plot()



spiral_racetrack_heater_metal
----------------------------------------------------

.. autofunction:: gdsfactory.components.spiral_racetrack_heater_metal

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.spiral_racetrack_heater_metal(straight_length=30, spacing=2, num=8, waveguide_cross_section='strip', heater_cross_section='heater_metal', via_stack='via_stack_heater_mtop')
  c.plot()



splitter_chain
----------------------------------------------------

.. autofunction:: gdsfactory.components.splitter_chain

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.splitter_chain(columns=3)
  c.plot()



splitter_tree
----------------------------------------------------

.. autofunction:: gdsfactory.components.splitter_tree

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.splitter_tree(noutputs=4, spacing=(90, 50), cross_section='strip')
  c.plot()



staircase
----------------------------------------------------

.. autofunction:: gdsfactory.components.staircase

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.staircase(length_v=5, length_h=5, rows=4)
  c.plot()



straight
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight(length=10, npoints=2, cross_section='strip')
  c.plot()



straight_array
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_array

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_array(n=4, spacing=4, length=10, cross_section='strip')
  c.plot()



straight_heater_doped_rib
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_doped_rib

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_doped_rib(length=320, nsections=3, via_stack_metal_size=(10, 10), via_stack_size=(10, 10), heater_width=2, heater_gap=0.8, via_stack_gap=0, width=0.5, xoffset_tip1=0.2, xoffset_tip2=0.4)
  c.plot()



straight_heater_doped_strip
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_doped_strip

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_doped_strip(length=320, nsections=3, via_stack_metal_size=(10, 10), via_stack_size=(10, 10), heater_width=2, heater_gap=0.8, via_stack_gap=0, width=0.5, xoffset_tip1=0.2, xoffset_tip2=0.4)
  c.plot()



straight_heater_meander
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_meander

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_meander(length=300, spacing=2, cross_section='strip', heater_width=2.5, extension_length=15, layer_heater='HEATER', radius=5, via_stack='via_stack_heater_mtop', heater_taper_length=10, straight_widths=(0.8, 0.9, 0.8), taper_length=10)
  c.plot()



straight_heater_meander_doped
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_meander_doped

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_meander_doped(length=300, spacing=2, cross_section='strip', heater_width=1.5, extension_length=15, layers_doping=('P', 'PP', 'PPP'), radius=5, straight_widths=(0.8, 0.9, 0.8), taper_length=10)
  c.plot()



straight_heater_metal
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_metal

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_metal(length=320, length_undercut_spacing=0, length_undercut=5, length_straight=0.1, length_straight_input=0.1, cross_section='strip', cross_section_heater='heater_metal', cross_section_waveguide_heater='strip_heater_metal', cross_section_heater_undercut='strip_heater_metal_undercut', with_undercut=False, via_stack='via_stack_heater_mtop', heater_taper_length=5)
  c.plot()



straight_heater_metal_90_90
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_metal_90_90

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_metal_90_90(length=320, length_undercut_spacing=0, length_undercut=5, length_straight=0.1, length_straight_input=0.1, cross_section='strip', cross_section_heater='heater_metal', cross_section_waveguide_heater='strip_heater_metal', cross_section_heater_undercut='strip_heater_metal_undercut', with_undercut=False, via_stack='via_stack_heater_mtop', port_orientation1=90, port_orientation2=90, heater_taper_length=5)
  c.plot()



straight_heater_metal_simple
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_metal_simple

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_metal_simple(length=320, cross_section_heater='heater_metal', cross_section_waveguide_heater='strip_heater_metal', via_stack='via_stack_heater_mtop', heater_taper_length=5)
  c.plot()



straight_heater_metal_undercut
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_metal_undercut

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_metal_undercut(length=320, length_undercut_spacing=6, length_undercut=30, length_straight=0.1, length_straight_input=15, cross_section='strip', cross_section_heater='heater_metal', cross_section_waveguide_heater='strip_heater_metal', cross_section_heater_undercut='strip_heater_metal_undercut', with_undercut=True, via_stack='via_stack_heater_mtop', heater_taper_length=5)
  c.plot()



straight_heater_metal_undercut_90_90
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_heater_metal_undercut_90_90

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_heater_metal_undercut_90_90(length=320, length_undercut_spacing=6, length_undercut=30, length_straight=0.1, length_straight_input=15, cross_section='strip', cross_section_heater='heater_metal', cross_section_waveguide_heater='strip_heater_metal', cross_section_heater_undercut='strip_heater_metal_undercut', with_undercut=True, via_stack='via_stack_heater_mtop', port_orientation1=90, port_orientation2=90, heater_taper_length=5)
  c.plot()



straight_pin
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_pin

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_pin(length=500, via_stack_width=10, via_stack_spacing=2)
  c.plot()



straight_pin_slot
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_pin_slot

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_pin_slot(length=500, cross_section='pin', via_stack='via_stack_m1_mtop', via_stack_width=10, via_stack_slab='via_stack_slab_m1_horizontal', via_stack_spacing=3, via_stack_slab_spacing=2, taper='taper_strip_to_ridge')
  c.plot()



straight_pn
----------------------------------------------------

.. autofunction:: gdsfactory.components.straight_pn

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.straight_pn(length=2000, via_stack_width=10, via_stack_spacing=2)
  c.plot()



switch_tree
----------------------------------------------------

.. autofunction:: gdsfactory.components.switch_tree

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.switch_tree(noutputs=4, spacing=(500, 100), cross_section='strip')
  c.plot()



taper
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper(length=10, width1=0.5, with_two_ports=True, cross_section='strip', port_names=('o1', 'o2'), port_types=('optical', 'optical'), with_bbox=True)
  c.plot()



taper2
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper2

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper2(length=10, width1=0.5, width2=3, with_two_ports=True, cross_section='strip', port_names=('o1', 'o2'), port_types=('optical', 'optical'), with_bbox=True)
  c.plot()



taper_adiabatic
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_adiabatic

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_adiabatic(width1=0.5, width2=5, length=0, alpha=1, wavelength=1.55, npoints=200, cross_section='strip')
  c.plot()



taper_cross_section
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_cross_section

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_cross_section(cross_section1='strip_rib_tip', cross_section2='rib2', length=10, npoints=100, linear=False, width_type='sine')
  c.plot()



taper_cross_section_linear
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_cross_section_linear

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_cross_section_linear(cross_section1='strip_rib_tip', cross_section2='rib2', length=10, npoints=2, linear=True, width_type='sine')
  c.plot()



taper_cross_section_parabolic
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_cross_section_parabolic

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_cross_section_parabolic(cross_section1='strip_rib_tip', cross_section2='rib2', length=10, npoints=101, linear=False, width_type='parabolic')
  c.plot()



taper_cross_section_sine
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_cross_section_sine

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_cross_section_sine(cross_section1='strip_rib_tip', cross_section2='rib2', length=10, npoints=101, linear=False, width_type='sine')
  c.plot()



taper_from_csv
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_from_csv

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_from_csv(cross_section='strip')
  c.plot()



taper_parabolic
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_parabolic

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_parabolic(length=20, width1=0.5, width2=5, exp=0.5, npoints=100, layer='WG')
  c.plot()



taper_sc_nc
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_sc_nc

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_sc_nc(length=20, width1=0.5, width2=0.15, w_slab1=0.15, w_slab2=1, layer_wg='WG', layer_slab='WGN', cross_section='strip', use_slab_port=True)
  c.plot()



taper_strip_to_ridge
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_strip_to_ridge

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_strip_to_ridge(length=10, width1=0.5, width2=0.5, w_slab1=0.15, w_slab2=6, layer_wg='WG', layer_slab='SLAB90', cross_section='strip', use_slab_port=False)
  c.plot()



taper_strip_to_ridge_trenches
----------------------------------------------------

.. autofunction:: gdsfactory.components.taper_strip_to_ridge_trenches

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.taper_strip_to_ridge_trenches(length=10, width=0.5, slab_offset=3, trench_width=2, trench_layer='DEEP_ETCH', layer_wg='WG', trench_offset=0.1)
  c.plot()



terminator
----------------------------------------------------

.. autofunction:: gdsfactory.components.terminator

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.terminator(length=50, tapered_width=0.2, doping_layers=('NPP',), doping_offset=1)
  c.plot()



text
----------------------------------------------------

.. autofunction:: gdsfactory.components.text

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.text(text='abcd', size=10, position=(0, 0), justify='left', layer='WG')
  c.plot()



text_freetype
----------------------------------------------------

.. autofunction:: gdsfactory.components.text_freetype

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.text_freetype(text='abcd', size=10, justify='left', layer='WG')
  c.plot()



text_klayout
----------------------------------------------------

.. autofunction:: gdsfactory.components.text_klayout

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.text_klayout(text='a', layer='WG')
  c.plot()



text_lines
----------------------------------------------------

.. autofunction:: gdsfactory.components.text_lines

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.text_lines(text=('Chip', '01'), size=0.4, layer='WG')
  c.plot()



text_rectangular
----------------------------------------------------

.. autofunction:: gdsfactory.components.text_rectangular

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.text_rectangular(text='abcd', size=10, position=(0, 0), justify='left', layer='WG')
  c.plot()



text_rectangular_mini
----------------------------------------------------

.. autofunction:: gdsfactory.components.text_rectangular_mini

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.text_rectangular_mini(text='abcd', size=1, position=(0, 0), justify='left', layer='WG')
  c.plot()



text_rectangular_multi_layer
----------------------------------------------------

.. autofunction:: gdsfactory.components.text_rectangular_multi_layer

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.text_rectangular_multi_layer(text='abcd', layers=('WG', 'M1', 'M2', 'MTOP'))
  c.plot()



triangle
----------------------------------------------------

.. autofunction:: gdsfactory.components.triangle

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.triangle(x=10, xtop=0, y=20, ybot=0, layer='WG')
  c.plot()



verniers
----------------------------------------------------

.. autofunction:: gdsfactory.components.verniers

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.verniers(widths=(0.1, 0.2, 0.3, 0.4, 0.5), gap=0.1, xsize=100, layer_label='TEXT')
  c.plot()



version_stamp
----------------------------------------------------

.. autofunction:: gdsfactory.components.version_stamp

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.version_stamp(labels=('demo_label',), with_qr_code=False, layer='WG', pixel_size=1, text_size=10)
  c.plot()



via_chain
----------------------------------------------------

.. autofunction:: gdsfactory.components.via_chain

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.via_chain(num_vias=100, cols=10, layers_bot=('M1',), layers_top=('M2',), offsets_top=(0,), offsets_bot=(0,), via_min_enclosure=1, min_metal_spacing=1)
  c.plot()



via_corner
----------------------------------------------------

.. autofunction:: gdsfactory.components.via_corner

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.via_corner(cross_section=(({'function': 'cross_section', 'settings': {'layer': 'M2', 'width': 10, 'port_names': ('e1', 'e2'), 'port_types': ('electrical', 'electrical'), 'radius': None}, 'module': 'gdsfactory.cross_section'}, (0, 180)), ({'function': 'cross_section', 'settings': {'layer': 'M3', 'width': 10, 'port_names': ('e1', 'e2'), 'port_types': ('electrical', 'electrical'), 'radius': None}, 'module': 'gdsfactory.cross_section'}, (90, 270))), layers_labels=('m2', 'm3'))
  c.plot()



via_stack
----------------------------------------------------

.. autofunction:: gdsfactory.components.via_stack

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.via_stack(size=(11, 11), layers=('M1', 'M2', 'MTOP'), correct_size=True, slot_horizontal=False, slot_vertical=False)
  c.plot()



via_stack_m1_mtop
----------------------------------------------------

.. autofunction:: gdsfactory.components.via_stack_m1_mtop

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.via_stack_m1_mtop(size=(11, 11), layers=('M1', 'M2', 'MTOP'), correct_size=True, slot_horizontal=False, slot_vertical=False)
  c.plot()



via_stack_npp_m1
----------------------------------------------------

.. autofunction:: gdsfactory.components.via_stack_npp_m1

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.via_stack_npp_m1(size=(11, 11), layers=('WG', 'NPP', 'M1'), correct_size=True, slot_horizontal=False, slot_vertical=False)
  c.plot()



via_stack_slab_m1_horizontal
----------------------------------------------------

.. autofunction:: gdsfactory.components.via_stack_slab_m1_horizontal

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.via_stack_slab_m1_horizontal(size=(11, 11), layers=('SLAB90', 'M1'), correct_size=True, slot_horizontal=True, slot_vertical=False)
  c.plot()



via_stack_with_offset
----------------------------------------------------

.. autofunction:: gdsfactory.components.via_stack_with_offset

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.via_stack_with_offset(layers=('PPP', 'M1'), size=(10, 10))
  c.plot()



wafer
----------------------------------------------------

.. autofunction:: gdsfactory.components.wafer

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.wafer(cols=(2, 6, 6, 8, 8, 6, 6, 2), die_name_col_row=False)
  c.plot()



wire_corner
----------------------------------------------------

.. autofunction:: gdsfactory.components.wire_corner

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.wire_corner(cross_section='metal_routing')
  c.plot()



wire_corner45
----------------------------------------------------

.. autofunction:: gdsfactory.components.wire_corner45

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.wire_corner45(cross_section='metal_routing', radius=10)
  c.plot()



wire_straight
----------------------------------------------------

.. autofunction:: gdsfactory.components.wire_straight

.. plot::
  :include-source:

  import gdsfactory as gf

  c = gf.components.wire_straight(length=10, npoints=2, cross_section='metal_routing')
  c.plot()
