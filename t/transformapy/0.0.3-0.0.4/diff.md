# Comparing `tmp/transformapy-0.0.3.zip` & `tmp/transformapy-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,8 @@
-Zip file size: 23089 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-06 21:37 transformapy-0.0.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-06 21:37 transformapy-0.0.3/transformapy.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-06 21:37 transformapy-0.0.3/transformapy/
--rw-r--r--  2.0 unx     3881 b- defN 24-Mar-06 21:37 transformapy-0.0.3/PKG-INFO
--rwx------  2.0 unx      743 b- defN 24-Mar-06 17:17 transformapy-0.0.3/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-06 21:37 transformapy-0.0.3/setup.cfg
--rwx------  2.0 unx     2683 b- defN 24-Mar-06 17:16 transformapy-0.0.3/README.rst
--rw-r--r--  2.0 unx     3881 b- defN 24-Mar-06 21:37 transformapy-0.0.3/transformapy.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      217 b- defN 24-Mar-06 21:37 transformapy-0.0.3/transformapy.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-06 21:37 transformapy-0.0.3/transformapy.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-06 21:37 transformapy-0.0.3/transformapy.egg-info/dependency_links.txt
--rwx------  2.0 unx      737 b- defN 24-Mar-06 17:09 transformapy-0.0.3/transformapy/__init__.py
--rwx------  2.0 unx    63414 b- defN 24-Mar-06 21:35 transformapy-0.0.3/transformapy/transformapy.py
-13 files, 75608 bytes uncompressed, 21061 bytes compressed:  72.1%
+Zip file size: 21774 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      892 b- defN 24-Apr-09 02:48 transformapy/__init__.py
+-rw-r--r--  2.0 unx    71862 b- defN 24-Apr-09 02:45 transformapy/transformapy.py
+-rw-r--r--  2.0 unx     4302 b- defN 24-Apr-09 08:06 transformapy-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 08:06 transformapy-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-09 08:06 transformapy-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      484 b- defN 24-Apr-09 08:06 transformapy-0.0.4.dist-info/RECORD
+6 files, 77645 bytes uncompressed, 20896 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -1,40 +1,19 @@
-Filename: transformapy-0.0.3/
+Filename: transformapy/__init__.py
 Comment: 
 
-Filename: transformapy-0.0.3/transformapy.egg-info/
+Filename: transformapy/transformapy.py
 Comment: 
 
-Filename: transformapy-0.0.3/transformapy/
+Filename: transformapy-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: transformapy-0.0.3/PKG-INFO
+Filename: transformapy-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: transformapy-0.0.3/setup.py
+Filename: transformapy-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: transformapy-0.0.3/setup.cfg
-Comment: 
-
-Filename: transformapy-0.0.3/README.rst
-Comment: 
-
-Filename: transformapy-0.0.3/transformapy.egg-info/PKG-INFO
-Comment: 
-
-Filename: transformapy-0.0.3/transformapy.egg-info/SOURCES.txt
-Comment: 
-
-Filename: transformapy-0.0.3/transformapy.egg-info/top_level.txt
-Comment: 
-
-Filename: transformapy-0.0.3/transformapy.egg-info/dependency_links.txt
-Comment: 
-
-Filename: transformapy-0.0.3/transformapy/__init__.py
-Comment: 
-
-Filename: transformapy-0.0.3/transformapy/transformapy.py
+Filename: transformapy-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `transformapy-0.0.3/PKG-INFO` & `transformapy-0.0.4.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,114 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: transformapy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
 Home-page: https://github.com/WangRui5/TransformaPy
 Author: Wang Rui
 Author-email: wtrt7009@gmail.com
 License: UNKNOWN
-Description: transformapy: A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
-        ==================================================================================================================
-        
-        transformapy is a Python toolkit engineered to process molecular structures, pinpointing potential transformation products of specified compounds by leveraging observed monoisotopic masses.
-        
-        Contributor: Rui Wang
-        =====================
-        
-        First release date: Feb.28.2024
-        
-        Update
-        ======
-        
-        Mar.09.2024: transformapy 0.0.3
-        
-        - fix some bugs;
-        - add some new functions. i.e., combine_two_frags, draw_molecule_with_atom_indices
-        
-        Dependencies
-        ============
-        
-        transformapy requires the following major dependencies:
-        
-        - rdkit
-        - pyhrms
-        
-        Features
-        ========
-        
-        transformapy provides the following functions:
-        
-        - Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
-        
-        Paper Published Utilizing transformapy
-        =======================================
-        
-        - Preparing
-        
-        Licensing
-        =========
-        
-        The package is open source and can be utilized under the MIT license. Please find the detail in the license file.
-        
-        transformapy Documentation
-        ===========================
-        
-        **Getting Started with transformapy**
-        
-        .. code-block:: python
-        
-            from transformapy.transformapy import *
-        
-        **Project Structure:**
-        
-        .. code-block:: none
-        
-            transformapy/
-            |- generate_possible_TP_structures
-               |- modify_chemical_formula
-               |- generate_fragments
-               |- calculate_formula_differences
-               |- combine_two_frags
-               |- calculate_changed_num
-                  |- parse_formula
-               |- recursive_reaction
-                  |- reaction_type
-                     |- combine_fragments_and_generate_smiles
-                     |- replace_dummies_with_hydrogens
-                     |- replace_hydrogen_with_substituent
-                     |- split_molecule_at_bond
-                     |- Remove_2H
-                        |- is_atom_in_double_bond
-                        |- add_or_modify_bond
-                        |- has_hydrogen_count
-                     |- Add_2H
-            |- remove_explicit_hydrogens
-            |- draw_molecule_with_atom_indices
-            |- GetIdxOfDummy
-            |- adjust_valence_by_removing_hydrogen
-        
-        Acknowledgment
-        ==============
-        
-        During the development of this package, Liu Huangrui from the South China Institute of Environmental Science offered essential support by conducting comprehensive tests on its functionality.
-        
-        Note
-        ====
-        
-        Please note that the documentation is currently a work in progress, and there is more content that is being written. I apologize for any inconvenience this may cause, but rest assured that I am continually updating the documentation to provide you with the most comprehensive guide to using transformapy.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
+
+transformapy: A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
+==================================================================================================================
+
+transformapy is a Python toolkit engineered to process molecular structures, pinpointing potential transformation products of specified compounds by leveraging observed monoisotopic masses.
+
+Contributor: Rui Wang
+=====================
+
+First release date: Feb.28.2024
+
+Update
+======
+
+April.09.2024: transformapy 0.0.4
+
+1. **Updated `remove_2H` Function**: Modifications have been made to improve the performance and accuracy of the `remove_2H` function.
+2. **New Helper Functions**: Added `check_bad_valance_Hidx` and `remove_additional_H` functions, which are now utilized internally by `remove_2H` to enhance its functionality.
+3. **Added `add_missing_H` Function**: Introduced a new function to automatically add missing hydrogen atoms to molecules to correct their valency.
+4. **Enhanced `reaction_type` Checks**: Integrated the `add_missing_H` and `remove_additional_H` functions into the `reaction_type` function to ensure molecule structures are correctly adjusted during reactions.
+5. **Introduced `stepwise_reaction` Function**: A new function to facilitate the stepwise application of reaction steps on a target molecule, allowing more detailed control over complex reaction pathways.
+6. **Improvements to `generate_possible_TP_structures`**: Significant updates have been made to this function to optimize the generation of possible transformation product structures based on modified chemical reaction processes.
+
+
+Dependencies
+============
+
+transformapy requires the following major dependencies:
+
+- rdkit
+- pyhrms
+
+Features
+========
+
+transformapy provides the following functions:
+
+- Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
+
+Paper Published Utilizing transformapy
+=======================================
+
+- Preparing
+
+Licensing
+=========
+
+The package is open source and can be utilized under the MIT license. Please find the detail in the license file.
+
+transformapy Documentation
+===========================
+
+**Getting Started with transformapy**
+
+.. code-block:: python
+
+    from transformapy.transformapy import *
+
+**Project Structure:**
+
+.. code-block:: none
+
+    transformapy/
+    |- from_mass_to_formula
+    |- generate_possible_TP_structures
+       |- modify_chemical_formula
+       |- generate_fragments
+       |- calculate_formula_differences
+       |- combine_two_frags
+       |- calculate_changed_num
+          |- parse_formula
+       |- stepwise_reaction
+          |- reaction_type
+             |- combine_fragments_and_generate_smiles
+             |- replace_dummies_with_hydrogens
+             |- replace_hydrogen_with_substituent
+             |- split_molecule_at_bond
+             |- Remove_2H
+                |- is_atom_in_double_bond
+                |- add_or_modify_bond
+                |- has_hydrogen_count
+             |- Add_2H
+             |- remove_additional_H
+                |- check_bad_valance_Hidx
+             |- add_missing_H
+    |- remove_explicit_hydrogens
+    |- draw_molecule_with_atom_indices
+    |- GetIdxOfDummy
+    |- adjust_valence_by_removing_hydrogen
+
+Acknowledgment
+==============
+
+During the development of this package, Liu Huangrui from the South China Institute of Environmental Science offered essential support by conducting comprehensive tests on its functionality.
+
+Note
+====
+
+Please note that the documentation is currently a work in progress, and there is more content that is being written. I apologize for any inconvenience this may cause, but rest assured that I am continually updating the documentation to provide you with the most comprehensive guide to using transformapy.
+
+
```

## Comparing `transformapy-0.0.3/transformapy/__init__.py` & `transformapy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import transformapy
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 __all__ = [
     "generate_possible_TP_structures",
     "modify_chemical_formula",
     "generate_fragments",
     "split_peak_picking",
     "calculate_formula_differences",
@@ -20,10 +20,15 @@
     "add_or_modify_bond",
     "has_hydrogen_count",
     "Add_2H",
     "combine_two_frags",
     "draw_molecule_with_atom_indices",
     "remove_explicit_hydrogens",
     "GetIdxOfDummy",
-    "adjust_valence_by_removing_hydrogen"
-    
+    "adjust_valence_by_removing_hydrogen",
+    "add_missing_H",
+    "check_bad_valance_Hidx",
+    "remove_additional_H",
+    "stepwise_reaction",
+    "from_mass_to_formula",
+    "is_valid_formula"
 ]
```

## Comparing `transformapy-0.0.3/transformapy/transformapy.py` & `transformapy/transformapy.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,346 @@
 import itertools
 import re
 from rdkit.Chem.Draw import rdMolDraw2D
 from IPython.display import SVG
 import rdkit
 from pyhrms.pyhrms import *
 
+
+def add_missing_H(mol):
+    """
+    Adds missing hydrogen atoms to the first encountered under-saturated carbon (C), nitrogen (N),
+    or oxygen (O) atom in a given molecule. This function is designed to ensure that these atoms reach
+    their typical valency: C (up to 4), N (up to 3), and O (up to 2).
+
+    Parameters:
+    - mol (Chem.Mol): The RDKit molecule object that will be modified. This molecule should be in a format
+                      that allows for valency checks and modifications.
+
+    Returns:
+    - Chem.Mol: The molecule with hydrogens added to the first found under-saturated atom of type C, N, or O.
+                Hydrogens are added only to the first such atom encountered that needs them to reach standard valency.
+
+    This function processes the input molecule by initially adding explicit hydrogens to all atoms. It then checks
+    each atom's type and current valency. If it finds an atom that is under-saturated (C, N, or O), it converts the
+    molecule to an editable format, adds a hydrogen atom, and forms a single bond. This modification stops after
+    correcting the first such atom found. Finally, it converts all hydrogens back to the implicit representation.
+    """
+
+    mol = Chem.AddHs(mol)
+    for atom in mol.GetAtoms():
+
+        if (atom.GetSymbol() == 'C' and atom.GetExplicitValence() < 4):
+            mol = Chem.EditableMol(mol)
+            h_idx = mol.AddAtom(Chem.Atom(1))
+            mol.AddBond(atom.GetIdx(), h_idx, Chem.BondType.SINGLE)
+            mol = mol.GetMol()
+            break
+        if (atom.GetSymbol() == 'N' and atom.GetExplicitValence() < 3):
+            mol = Chem.EditableMol(mol)
+            h_idx = mol.AddAtom(Chem.Atom(1))
+            mol.AddBond(atom.GetIdx(), h_idx, Chem.BondType.SINGLE)
+            mol = mol.GetMol()
+            break
+        if (atom.GetSymbol() == 'O' and atom.GetExplicitValence() < 2):
+            mol = Chem.EditableMol(mol)
+            h_idx = mol.AddAtom(Chem.Atom(1))
+            mol.AddBond(atom.GetIdx(), h_idx, Chem.BondType.SINGLE)
+            mol = mol.GetMol()
+            break
+
+    mol = Chem.RemoveHs(mol)
+    return mol
+
+
+def check_bad_valance_Hidx(test1):
+    """
+    Adds missing hydrogen atoms to under-saturated carbon (C), nitrogen (N), or oxygen (O) atoms in a molecule.
+    This function first adds explicit hydrogen atoms to all potential sites, then specifically targets the first
+    under-saturated C, N, or O found and manually adjusts their hydrogen count to satisfy typical valency rules:
+    C (valency up to 4), N (up to 3), O (up to 2).
+
+    Parameters:
+    - mol (Chem.Mol): An RDKit molecule object that potentially has under-saturated atoms.
+
+    Returns:
+    - Chem.Mol: The modified molecule with added hydrogen atoms, ensuring that the valency rules are met for C, N, and O.
+
+    The function modifies the molecule by adding hydrogen atoms to reach the standard valency and then reverts to
+    implicit hydrogen representation. It will stop and return after modifying the first eligible atom found.
+    """
+    H_idx = []
+    for atom in test1.GetAtoms():
+        if atom.GetSymbol() == 'C':
+            if atom.GetExplicitValence() > 4:
+                for bond in atom.GetBonds():
+                    if bond.GetOtherAtom(atom).GetSymbol() == 'H':
+                        H_idx.append(bond.GetOtherAtom(atom).GetIdx())
+                        break
+    for atom in test1.GetAtoms():
+        if atom.GetSymbol() == 'N':
+            if atom.GetExplicitValence() > 3:
+                for bond in atom.GetBonds():
+                    if bond.GetOtherAtom(atom).GetSymbol() == 'H':
+                        H_idx.append(bond.GetOtherAtom(atom).GetIdx())
+                        break
+    for atom in test1.GetAtoms():
+        if atom.GetSymbol() == 'O':
+            if atom.GetExplicitValence() > 2:
+                for bond in atom.GetBonds():
+                    if bond.GetOtherAtom(atom).GetSymbol() == 'H':
+                        H_idx.append(bond.GetOtherAtom(atom).GetIdx())
+                        break
+    return H_idx
+
+
+# Check the valence
+def remove_additional_H(modified_mol):
+    """
+    Removes two hydrogen atoms from a molecule where a single bond has been transformed into a double bond.
+    This function identifies hydrogen atoms that are incorrectly maintaining single bonds where double bonds
+    should exist due to a previous modification. It removes these hydrogen atoms to correct the molecular structure.
+
+    Parameters:
+    - modified_mol (Chem.Mol): An RDKit molecule object potentially containing incorrect single bonds due
+                               to improperly placed hydrogen atoms after a structural modification.
+
+    Returns:
+    - Chem.Mol: The modified molecule with excess hydrogens removed and the molecular structure corrected to
+                accurately reflect the intended valency and bonding.
+
+    The function first adds explicit hydrogens to identify any incorrectly bonded hydrogen atoms. It then iteratively
+    removes these atoms, one at a time, until the structure adheres to proper valency rules. The molecule is sanitized
+    to update its chemical properties after the removals.
+    """
+    test1 = Chem.AddHs(modified_mol)
+    bad_Hidx = check_bad_valance_Hidx(test1)
+    if len(bad_Hidx) == 0:
+        test1 = modified_mol
+    else:
+        test1 = Chem.EditableMol(test1)  # 转换成可以编辑的结构
+        test1.RemoveAtom(bad_Hidx[0])
+        test1 = test1.GetMol()  # 重新获得新的结构
+        bad_Hidx = check_bad_valance_Hidx(test1)  # 重新查找bad H idx
+        test1 = Chem.EditableMol(test1)
+        test1.RemoveAtom(bad_Hidx[-1])
+        test1 = test1.GetMol()  # 重新获得新的结构
+        test1 = Chem.RemoveHs(test1)
+        Chem.SanitizeMol(test1, Chem.SanitizeFlags.SANITIZE_PROPERTIES)
+
+    return test1
+
+
+def stepwise_reaction(target_mol, rxn_s1):
+    """
+    Performs a series of chemical reactions on a given molecule step-by-step, based on specified reaction types and counts.
+
+    Args:
+        target_mol (mol object): The molecule object that is subjected to the reactions.
+        rxn_s1 (dict): Dictionary mapping reaction types (keys) to their respective counts (values).
+            Positive counts indicate forward reactions, and negative counts indicate reverse reactions.
+
+    Returns:
+        list: A list of molecule objects that represent the potential outcomes after applying all specified reactions stepwise.
+
+    The function executes each reaction as specified in 'rxn_s1', starting from 'target_mol'. If the sequence of reactions is longer than three steps, a prompt is printed to simplify the reactions or break them into manageable steps.
+    """
+    final_tps = []
+    # 1. 先把有多少步反应讲清楚
+    dict1 = rxn_s1
+    keys_list = []
+    values_list = []
+    for key, value in dict1.items():
+        if value > 0:
+            keys_list.extend([key] * value)
+            values_list.extend([1] * value)
+        elif value < 0:
+            keys_list.extend([key] * abs(value))
+            values_list.extend([-1] * abs(value))
+
+    # 2. 再一步步进行解析
+    if len(keys_list) >= 1:
+        tps1 = reaction_type(target_mol, rxn_type=keys_list[0], num=values_list[0])
+        if len(keys_list) == 1:
+            final_tps.extend(tps1)  # 如果只有一步就直接extend了
+        else:
+            # 继续第二步
+            tps2 = []
+            for tp1 in tps1:
+                tps2_ = reaction_type(tp1, rxn_type=keys_list[1], num=values_list[1])  # 第二步了，所以都是【1】
+                tps2.extend(tps2_)
+            # 判断是不是只有两步
+            if len(keys_list) == 2:
+                final_tps.extend(tps2)
+            else:
+                # 继续第三步
+                tps3 = []
+                for tp2 in tps2:
+                    tp3_ = reaction_type(tp2, rxn_type=keys_list[2], num=values_list[2])
+                    tps3.extend(tp3_)
+                if len(keys_list) == 3:
+                    final_tps.extend(tps3)
+                else:
+                    print('Please simplify the reaction or break it down into multiple steps.')
+    return final_tps
+
+
+def generate_possible_TP_structures(parent_mol, TP_formula, mode='pos'):
+    """
+    Generates possible transformation product (TP) structures by modifying a parent molecule
+    based on a target transformation product formula and reaction mode.
+
+    This function identifies potential sites for modification in the parent molecule, applies
+    chemical transformations based on the specified target TP formula, and considers the reaction
+    mode (positive or negative ion mode) to adjust the molecular structure accordingly. The goal
+    is to explore plausible structural changes that align with the target TP formula, generating
+    a set of potential TP structures.
+
+    Parameters:
+    - parent_mol (Chem.Mol): The RDKit molecule object representing the parent molecule.
+    - TP_formula (str): The chemical formula of the target transformation product.
+    - mode (str, optional): The ionization mode, either 'pos' for positive or 'neg' for negative.
+      Default is 'pos'. This affects how the molecular structure is adjusted to match the target
+      TP formula.
+
+    Returns:
+    - list of Chem.Mol: A list of RDKit molecule objects representing potential TP structures
+      that match the target TP formula.
+
+    Steps:
+    1. Identify atoms in the parent molecule that have hydrogen atoms available for substitution.
+    2. Adjust the target TP formula based on the reaction mode to account for ionization effects.
+    3. Compare the parent molecule's formula with the target TP formula to identify differences.
+    4. Fragment the parent molecule and evaluate each fragment for potential modifications.
+    5. Generate a series of reaction types based on the identified differences and apply these
+       to the parent molecule or its fragments to generate potential TP structures.
+
+    Note:
+    - The function assumes that the parent molecule and the target TP formula represent chemically
+      valid structures.
+    - The generated TP structures are theoretical and may require further validation to ensure
+      their chemical plausibility.
+    """
+
+    formula = CalcMolFormula(parent_mol)
+
+    possible_TPs = {}
+    # Step 0. 看看哪些原子上有H，这样可以取代
+    atoms_with_H = []
+    for atom in parent_mol.GetAtoms():
+        if has_hydrogen_count(atom):
+            atoms_with_H.append(atom.GetIdx())
+
+    # step 1. 根据正负离子模式转化成中性分子
+    if mode == 'pos':
+        TP_formula = modify_chemical_formula(TP_formula, '-H')
+    if mode == 'neg':
+        TP_formula = modify_chemical_formula(TP_formula, '+H')
+
+    # step 2. 对比一下和母体结构差异
+    structures_dict = {}  # 创建一个新的字典
+    reduced_part, added_part = calculate_formula_differences(formula, TP_formula)
+    num = calculate_changed_num(reduced_part, added_part)
+    structures_dict[parent_mol] = num
+
+    # Step 3. 打碎分子并存储
+    frags = generate_fragments(parent_mol)
+    frags = [replace_dummies_with_hydrogens(frag) for frag in frags]
+    frag_smis = list(set([Chem.MolToSmiles(frag) for frag in frags]))
+    frags1 = [Chem.MolFromSmiles(frag_smi) for frag_smi in frag_smis]
+
+    # Step 3.1 补充那些两两组合的
+    frags = generate_fragments(parent_mol)
+    pairs = list(itertools.combinations(list(np.arange(len(frags))), 2))
+    for pair in tqdm(pairs, desc='Combine different frags'):
+        mol1 = frags[pair[0]]
+        mol2 = frags[pair[1]]
+        new_mol = combine_two_frags(mol1, mol2)
+        frags1.append(new_mol)
+
+    # Step 4. 计算分子式总的改变个数,确定在哪个碎片上进行加工 (要重新写，考虑同样分子式的情况)
+
+    for frag in tqdm(frags1, desc='Finding the most relavent structure'):
+        frag_formula = CalcMolFormula(frag)
+        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula)
+        frag_total_num = calculate_changed_num(reduced_part, added_part)
+        structures_dict[frag] = frag_total_num
+
+    # Step 5. 将要修改的parent/frag与TP的分子式对比，生成series
+    sub_rxn = ['NH', 'O', 'CH2', 'H-1NO2', 'H2', 'H-1Cl', 'H-1Br', 'H-1F', 'H-1I']
+    s = pd.Series(structures_dict).sort_values()
+    s1 = s[s == s.min()]
+    target_mols = list(s1.index)
+    # 去除重复的
+    target_mols_smi = list(set([Chem.MolToSmiles(i) for i in target_mols]))
+    target_mols = [Chem.MolFromSmiles(i) for i in target_mols_smi]
+    for target_mol in target_mols:
+        print(f'First Step TP: {Chem.MolToSmiles(target_mol)}')
+        print(f'----------------------------------------------')
+        frag_formula = CalcMolFormula(target_mol)
+        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula)
+        print(f'reduced_part:{reduced_part}, added_part:{added_part}')
+        s1 = pd.Series(parse_formula(reduced_part), dtype=object) * -1
+        s2 = pd.Series(parse_formula(added_part), dtype=object)
+        change_s = pd.concat([s1, s2])
+        if len(change_s) == 0:  # 说明和碎片相同
+            possible_TPs[target_mol] = 'Frag'
+        else:
+            # 开始处理每个元素
+            atoms = ['C', 'H', 'O', 'N', 'Cl', 'Br', 'F', 'I']
+            atoms_not_present = [i for i in atoms if i not in change_s.index]
+            unpresent_s = pd.Series(np.zeros(len(atoms_not_present)).astype(int), atoms_not_present)
+            change_s1 = pd.concat([change_s, unpresent_s])
+            # 确定范围
+            ranges = [range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
+                      range(min([0, change_s1['O']]), max([0, change_s1['O']]) + 1),
+                      range(min([0, change_s1['C']]), max([0, change_s1['C']]) + 1),
+                      range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
+                      range(-5, 5),
+                      range(min([0, change_s1['Cl']]), max([0, change_s1['Cl']]) + 1),
+                      range(min([0, change_s1['Br']]), max([0, change_s1['Br']]) + 1),
+                      range(min([0, change_s1['F']]), max([0, change_s1['F']]) + 1),
+                      range(min([0, change_s1['I']]), max([0, change_s1['I']]) + 1)]
+            patterns_list = list(itertools.product(*ranges))
+            # 开始做匹配
+            rxn_s = None
+            for pattern in patterns_list:
+                a, b, c, d, e, f, g, h, i = pattern  # a*NH, b*O, c*CH2, d*H-1NO2, e*H2, f*H-1Cl, g*H-1Br, h*H-1F, i*H-1I
+                N_num = a + d  # a
+                O_num = b + 2 * d  # b
+                C_num = c  # c
+                Cl_num = f
+                Br_num = g
+                F_num = h
+                I_num = i
+                H_num = a + 2 * c - d + 2 * e - f - g - h - i
+                if (N_num == change_s1['N']) & (O_num == change_s1['O']) & (C_num == change_s1['C']) & (
+                        Cl_num == change_s1['Cl']) & (Br_num == change_s1['Br']) & (F_num == change_s1['F']) & (
+                        I_num == change_s1['I']) & (H_num == change_s1['H']):
+                    rxn_s = pd.Series([a, b, c, d, e, f, g, h, i], sub_rxn)
+                    # 开始处理该分子
+                    rxn_s1 = rxn_s[rxn_s != 0]  # 去掉那些没有用的
+                    rxn_s1 = pd.concat([rxn_s1[['H2']], rxn_s1.drop('H2')]) if 'H2' in rxn_s1.index else rxn_s1
+                    rxn_s1_dict = rxn_s1.to_dict()
+                    print(rxn_s1_dict)
+                    # 先关注第一步的结构
+                    print(Chem.MolToSmiles(target_mol))
+                    possible_tp_list = stepwise_reaction(target_mol, rxn_s1)
+
+                    for rxn_tp in possible_tp_list:
+                        possible_TPs[rxn_tp] = str(rxn_s1_dict)
+
+        print(f'===============================================')
+    tp_list = [k for k, v in possible_TPs.items()]
+    tp_list = [i for i in tp_list if CalcMolFormula(i) == TP_formula]  # 去掉不符合formula的
+    tp_smiles = list(set([Chem.MolToSmiles(i) for i in tp_list]))  # 去重
+    tp_list = [Chem.MolFromSmiles(i) for i in tp_smiles]
+    return tp_list
+
+
 def from_mass_to_formula(parent_mol, observed_mz, mode, iso_info, ms_error=10, iso_score=0.7, addition_element={}):
     """
     Convert an observed mass to a chemical formula based on a parent molecule and additional criteria.
 
     Args:
         parent_mol (Mol): The parent molecule (RDKit Mol object) from which to derive the formula.
         observed_mz (float): The observed mass/charge (m/z) ratio.
@@ -77,15 +409,15 @@
     # 对pos和neg下的分子式进行修改
     result1['formula_neutral'] = result1['formula'].apply(modify_chemical_formula,
                                                           args=['-H'] if mode == 'pos' else ['+H'])
 
     # 看看这些合理的分子式相对于母体的变化
     for i in range(len(result1)):
         formula = result1.loc[i, 'formula_neutral']
-        added_part, reduced_part = calculate_formula_differences(parent_formula, formula)
+        reduced_part, added_part = calculate_formula_differences(parent_formula, formula)
         result1.loc[i, 'added part'] = added_part
         result1.loc[i, 'reduced part'] = reduced_part
         result1.loc[i, 'Changed Num'] = int(calculate_changed_num(added_part, reduced_part))
         result1.loc[i, 'element Num'] = len(parse_formula(added_part)) + len(parse_formula(reduced_part))
         if isinstance(iso_info, dict):
             iso_score = isotope_score(iso_info, formula, mode=mode)
             result1.loc[i, 'iso_score'] = iso_score
@@ -227,163 +559,14 @@
                             emol.RemoveBond(atom1_idx, atom2_idx)
                             emol.RemoveAtom(H_idx)
                             break
                     break
     return emol.GetMol()
 
 
-def generate_possible_TP_structures(parent_mol, TP_formula, mode='pos'):
-    """
-    Generates possible transformation product (TP) structures by modifying a parent molecule
-    based on a target transformation product formula and reaction mode.
-
-    This function identifies potential sites for modification in the parent molecule, applies
-    chemical transformations based on the specified target TP formula, and considers the reaction
-    mode (positive or negative ion mode) to adjust the molecular structure accordingly. The goal
-    is to explore plausible structural changes that align with the target TP formula, generating
-    a set of potential TP structures.
-
-    Parameters:
-    - parent_mol (Chem.Mol): The RDKit molecule object representing the parent molecule.
-    - TP_formula (str): The chemical formula of the target transformation product.
-    - mode (str, optional): The ionization mode, either 'pos' for positive or 'neg' for negative.
-      Default is 'pos'. This affects how the molecular structure is adjusted to match the target
-      TP formula.
-
-    Returns:
-    - list of Chem.Mol: A list of RDKit molecule objects representing potential TP structures
-      that match the target TP formula.
-
-    Steps:
-    1. Identify atoms in the parent molecule that have hydrogen atoms available for substitution.
-    2. Adjust the target TP formula based on the reaction mode to account for ionization effects.
-    3. Compare the parent molecule's formula with the target TP formula to identify differences.
-    4. Fragment the parent molecule and evaluate each fragment for potential modifications.
-    5. Generate a series of reaction types based on the identified differences and apply these
-       to the parent molecule or its fragments to generate potential TP structures.
-
-    Note:
-    - The function assumes that the parent molecule and the target TP formula represent chemically
-      valid structures.
-    - The generated TP structures are theoretical and may require further validation to ensure
-      their chemical plausibility.
-    """
-
-    formula = CalcMolFormula(parent_mol)
-
-    possible_TPs = {}
-    # Step 0. 看看哪些原子上有H，这样可以取代
-    atoms_with_H = []
-    for atom in parent_mol.GetAtoms():
-        if has_hydrogen_count(atom):
-            atoms_with_H.append(atom.GetIdx())
-
-    # step 1. 根据正负离子模式转化成中性分子
-    if mode == 'pos':
-        TP_formula = modify_chemical_formula(TP_formula, '-H')
-    if mode == 'neg':
-        TP_formula = modify_chemical_formula(TP_formula, '+H')
-
-    # step 2. 对比一下和母体结构差异
-    structures_dict = {}  # 创建一个新的字典
-    reduced_part, added_part = calculate_formula_differences(formula, TP_formula)
-    num = calculate_changed_num(reduced_part, added_part)
-    structures_dict[parent_mol] = num
-
-    # Step 3. 打碎分子并存储
-    frags = generate_fragments(parent_mol)
-    frags = [replace_dummies_with_hydrogens(frag) for frag in frags]
-    frag_smis = list(set([Chem.MolToSmiles(frag) for frag in frags]))
-    frags1 = [Chem.MolFromSmiles(frag_smi) for frag_smi in frag_smis]
-
-    # Step 3.1 补充那些两两组合的
-    frags = generate_fragments(parent_mol)
-    pairs = list(itertools.combinations(list(np.arange(len(frags))), 2))
-    for pair in tqdm(pairs, desc='Combine different frags'):
-        mol1 = frags[pair[0]]
-        mol2 = frags[pair[1]]
-        new_mol = combine_two_frags(mol1, mol2)
-        frags1.append(new_mol)
-
-    # Step 4. 计算分子式总的改变个数,确定在哪个碎片上进行加工 (要重新写，考虑同样分子式的情况)
-
-    for frag in tqdm(frags1, desc='Finding the most relavent structure'):
-        frag_formula = CalcMolFormula(frag)
-        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula)
-        frag_total_num = calculate_changed_num(reduced_part, added_part)
-        structures_dict[frag] = frag_total_num
-
-    # Step 5. 将要修改的parent/frag与TP的分子式对比，生成series
-    sub_rxn = ['NH', 'O', 'CH2', 'H-1NO2', 'H2', 'H-1Cl', 'H-1Br', 'H-1F', 'H-1I']
-    s = pd.Series(structures_dict).sort_values()
-    s1 = s[s == s.min()]
-    target_mols = list(s1.index)
-    # 去除重复的
-    target_mols_smi = list(set([Chem.MolToSmiles(i) for i in target_mols]))
-    target_mols = [Chem.MolFromSmiles(i) for i in target_mols_smi]
-    for target_mol in target_mols:
-        print(f'First Step TP: {Chem.MolToSmiles(target_mol)}')
-        print(f'----------------------------------------------')
-        frag_formula = CalcMolFormula(target_mol)
-        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula)
-        print(f'reduced_part:{reduced_part}, added_part:{added_part}')
-        s1 = pd.Series(parse_formula(reduced_part), dtype=object) * -1
-        s2 = pd.Series(parse_formula(added_part), dtype=object)
-        change_s = pd.concat([s1, s2])
-        if len(change_s) == 0:  # 说明和碎片相同
-            possible_TPs[target_mol] = 'Frag'
-        else:
-            # 开始处理每个元素
-            atoms = ['C', 'H', 'O', 'N', 'Cl', 'Br', 'F', 'I']
-            atoms_not_present = [i for i in atoms if i not in change_s.index]
-            unpresent_s = pd.Series(np.zeros(len(atoms_not_present)).astype(int), atoms_not_present)
-            change_s1 = pd.concat([change_s, unpresent_s])
-            # 确定范围
-            ranges = [range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
-                      range(min([0, change_s1['O']]), max([0, change_s1['O']]) + 1),
-                      range(min([0, change_s1['C']]), max([0, change_s1['C']]) + 1),
-                      range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
-                      range(-5, 5),
-                      range(min([0, change_s1['Cl']]), max([0, change_s1['Cl']]) + 1),
-                      range(min([0, change_s1['Br']]), max([0, change_s1['Br']]) + 1),
-                      range(min([0, change_s1['F']]), max([0, change_s1['F']]) + 1),
-                      range(min([0, change_s1['I']]), max([0, change_s1['I']]) + 1)]
-            patterns_list = list(itertools.product(*ranges))
-            # 开始做匹配
-            rxn_s = None
-            for pattern in patterns_list:
-                a, b, c, d, e, f, g, h, i = pattern  # a*NH, b*O, c*CH2, d*H-1NO2, e*H2, f*H-1Cl, g*H-1Br, h*H-1F, i*H-1I
-                N_num = a + d  # a
-                O_num = b + 2 * d  # b
-                C_num = c  # c
-                Cl_num = f
-                Br_num = g
-                F_num = h
-                I_num = i
-                H_num = a + 2 * c - d + 2 * e - f - g - h - i
-                if (N_num == change_s1['N']) & (O_num == change_s1['O']) & (C_num == change_s1['C']) & (
-                        Cl_num == change_s1['Cl']) & (Br_num == change_s1['Br']) & (F_num == change_s1['F']) & (
-                        I_num == change_s1['I']) & (H_num == change_s1['H']):
-                    rxn_s = pd.Series([a, b, c, d, e, f, g, h, i], sub_rxn)
-                    # 开始处理该分子
-                    rxn_s1 = rxn_s[rxn_s != 0]  # 去掉那些没有用的
-                    rxn_s1 = pd.concat([rxn_s1[['H2']], rxn_s1.drop('H2')]) if 'H2' in rxn_s1.index else rxn_s1
-                    rxn_s1_dict = rxn_s1.to_dict()
-                    print(rxn_s1_dict)
-                    # 先关注第一步的结构
-                    print(Chem.MolToSmiles(target_mol))
-                    possible_tp_list = recursive_reaction([target_mol], rxn_s1, current_step=0, possible_TPs=[])
-                    for rxn_tp in possible_tp_list:
-                        possible_TPs[rxn_tp] = str(rxn_s1_dict)
-
-        print(f'===============================================')
-
-    return possible_TPs
-
-
 def generate_fragments(mol):
     """
     Generates molecular fragments by breaking each single bond in the molecule.
 
     This function iterates over all the bonds in a given molecule and, for each single bond,
     creates a new set of fragments by breaking that bond. The process is repeated for all single
     bonds, and the resulting fragments are collected. Each fragment is treated as a separate molecule.
@@ -704,17 +887,15 @@
     and then constructs new formulas representing the excess elements in each original formula.
 
     Parameters:
     - formula1 (str): The first chemical formula as a string.
     - formula2 (str): The second chemical formula as a string.
 
     Returns:
-    - tuple: A tuple containing two strings:
-        - The first string represents the excess elements in `formula1` relative to `formula2`.
-        - The second string represents the excess elements in `formula2` relative to `formula1`.
+    - reduced_part, added_part
 
     Example:
     >>> calculate_formula_differences('H2O', 'H2O2')
     ('', 'O')
     >>> calculate_formula_differences('C6H12O6', 'C6H6')
     ('H6O6', '')
 
@@ -853,17 +1034,19 @@
             atom2 = mol.GetAtomWithIdx(idx2)
             # 如果两个原子上都有H原子，就可以相连
             if (has_hydrogen_count(atom1) & has_hydrogen_count(atom2) & (not is_atom_in_double_bond(atom1)) & (
                     not is_atom_in_double_bond(atom2))):
                 editable_mol = Chem.EditableMol(mol)
                 add_or_modify_bond(editable_mol, idx1, idx2, Chem.BondType.DOUBLE)
                 modified_mol = editable_mol.GetMol()
+                modified_mol = remove_additional_H(modified_mol)  # 去掉多余的H
                 Chem.SanitizeMol(modified_mol, Chem.SanitizeFlags.SANITIZE_PROPERTIES)
                 modified_smi = Chem.MolToSmiles(modified_mol)
                 new_smis.append(modified_smi)
+
     # 检查两两是否可以相连
     ring_info = mol.GetRingInfo()
     atoms_to_connect = []
     for atom in mol.GetAtoms():
         if has_hydrogen_count(atom):
             atoms_to_connect.append(atom.GetIdx())
 
@@ -882,15 +1065,15 @@
 
     for pair in possible_connections1:
         try:
             editable_mol = Chem.EditableMol(mol)
             add_or_modify_bond(editable_mol, pair[0], pair[1], Chem.BondType.SINGLE)
             # Convert back to a regular molecule
             modified_mol = editable_mol.GetMol()
-            modified_mol = Chem.RemoveHs(modified_mol)
+            modified_mol = remove_additional_H(modified_mol)
             Chem.SanitizeMol(modified_mol, Chem.SanitizeFlags.SANITIZE_PROPERTIES)
             modified_smi = Chem.MolToSmiles(modified_mol)
             new_smis.append(modified_smi)
         except Exception as e:
             print(f"Error with pair {pair}: {e}")
 
     # Step 2: 判断smiles是否合理
@@ -1170,14 +1353,16 @@
             for bond in C_NO2:
                 possible_TPs.extend(
                     [mol for mol in split_molecule_at_bond(mol, bond.GetIdx()) if CalcMolFormula(mol) != 'NO2'])
         if rxn_type == 'O':
             for bond in C_O:
                 possible_TPs.extend(
                     [mol for mol in split_molecule_at_bond(mol, bond.GetIdx()) if CalcMolFormula(mol) != 'H2O'])
+    possible_TPs = [add_missing_H(i) for i in possible_TPs]
+    possible_TPs = [remove_additional_H(i) for i in possible_TPs]
     return possible_TPs
 
 
 def remove_explicit_hydrogens(smiles):
     """
     Converts explicit hydrogen atoms in a molecule to implicit hydrogens.
```

