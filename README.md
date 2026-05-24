Gaussian2Plane: A Unified Coplanarity-Aware Framework for Compact Plane Extraction from 3D Gaussians


Planar primitives are fundamental geometric elements in man-made environments and play a crucial role in complex tasks such as 3D reconstruction, scene understanding, and robot navigation. Recent advances in 3D Gaussian Splatting (3DGS) have enabled high-quality scene synthesis and fine-grained 3D reconstruction, but deriving a compact set of geometrically faithful planes from 3D Gaussians remains challenging, as their unstructured representation provides no explicit surfaces. Existing methods primarily focus on local geometric fidelity, while plane set complexity is often insufficiently optimized, resulting in fragmented and redundant plane sets. This paper proposes Gaussian2Plane, a unified coplanarity-aware framework for compact plane extraction from 3D Gaussians. The key idea is to formulate plane extraction from 3DGS scenes as a differentiable optimization process that unifies 3DGS-rendered geometric supervision with coplanarity-aware structural regularization, enabling geometric fidelity and plane-set compactness to be optimized together. Our method first builds a planar primitive scaffold from an explicit point cloud fused from 3DGS-rendered depth maps, providing comprehensive planar coverage and structural priors for refinement. The planar primitives are then optimized through differentiable rendering under 3DGS-rendered depth and normal supervision to improve geometric consistency, while coplanarity loss and periodic identity-driven structural updates progressively consolidate fragmented primitives into coherent plane-level structures. Experiments on outdoor and indoor scenes show that our method produces more compact and complete plane sets than existing methods while maintaining comparable geometric accuracy, providing a reliable geometric basis for compact mesh reconstruction and scene understanding.
<img width="862" height="622" alt="image" src="https://github.com/user-attachments/assets/429b23aa-70dd-4baf-9df5-a52863217ff9" />




 Input city model
<img width="975" height="1395" alt="image" src="https://github.com/user-attachments/assets/bd88f208-9300-49d6-bb7e-cf8f4117b92f" />




Application in compact mesh reconstruction.
<img width="874" height="532" alt="image" src="https://github.com/user-attachments/assets/c1832d98-b8ff-4178-a54b-c32ca043bb77" />


Extension to point-cloud inputs and application in compact mesh reconstruction
<img width="526" height="572" alt="image" src="https://github.com/user-attachments/assets/73594d46-022b-4b9a-8999-6a73e13fb846" />




