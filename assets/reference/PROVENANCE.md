# Reference-cache provenance

The four `.npz` files contain raw `pred_logits` after sigmoid and normalized
`pred_boxes` produced on 24 August 2026 by the official CountGD code and
`checkpoint_fsc147_best.pth` (SHA-256
`c1bab864b17db345b4c6e3aaabb5765bc2c0a90d0bc8defb5e664a74a50aa126`).

| Cache | Image | Prompt mode | Expected count at 0.23 |
|---|---|---|---:|
| `women_girl_raw.npz` | `women.jpg` | text: `girl` | 5 |
| `car_text_raw.npz` | `car.jpg` | text: `car` | 16 |
| `car_exemplar_raw.npz` | `car.jpg` | one yellow-car exemplar | 16 |
| `car_multimodal_raw.npz` | `car.jpg` | text + the same exemplar | 16 |

The exemplar is `[55, 72, 151, 218]` in original-image pixel `xyxy` order.
The assessed tasks use these documented caches directly, so students do not
need the large checkpoint, BERT assets, or an external CountGD source tree.
